<script setup>
import { ref } from 'vue'
const addtask = ref('')
const Tasks = ref([])
const complete = ref(['harsh'])
const add = () => {
  if (addtask.value.trim() !== '') {
    Tasks.value.push(addtask.value)
    addtask.value = ' '
  }
}

const deleteTask = (index) => {
  Tasks.value.splice(index, 1)
}

const completed = (task, index) => {
  Tasks.value.splice(index, 1)
  complete.value.push(task)
}
</script>

<template>
  <main class="w-screen h-screen bg-black">
    <h1
      class="w-full p-5 text-xl font-semibold tracking-wide text-center text-yellow-500 uppercase transition-all bg-black border-b border-yellow-500 lg:text-4xl lg:p-10 hover:bg-yellow-500 hover:text-black"
    >
      Harsh Uleedri
    </h1>
    <p class="py-5 text-2xl font-semibold text-center text-white lg:py-10 lg:text-3xl">
      Today's Task
    </p>
    <div class="flex flex-col items-center justify-center w-full p-5 lg:p-10">
      <form @submit.prevent="newtask">
        <div class="flex flex-col items-center justify-center lg:flex-row">
          <input
            class="px-5 py-2 text-lg font-semibold border-2 focus:border-yellow-400"
            placeholder="Add Task"
            type="text"
            v-model="addtask"
          />
          <button
            type="submit"
            class="px-10 py-2 mt-5 text-lg font-semibold text-gray-900 bg-yellow-500 rounded-sm lg:mt-0 hover:bg-yellow-400 active:text-white"
            @click="add"
          >
            Add Task
          </button>
        </div>
      </form>
      <div class="flex items-center justify-center w-3/4 pt-5 lg:pt-10">
        <ul>
          <li
            class="flex justify-between px-3 py-3 text-base font-semibold bg-gray-300 border-b lg:px-10 lg:text-xl w-80 lg:w-full x-5 border-b-gray-400 text-wrap"
            v-for="(task, index) in Tasks"
            :key="task"
          >
            <span class="w-44">
              <p class="break-words">
                {{ task }}
              </p>
            </span>
            <span class="pl-3 lg:pl-10">
              <button
                class="px-3 py-1 text-xs text-white bg-green-500 rounded lg:px-5 lg:text-base"
                @click="completed(task, index)"
              >
                Complete
              </button>
              <button
                class="px-2 py-1 ml-1 text-xs font-semibold text-white bg-red-600 rounded-full lg:pb-1 lg:text-base lg:ml-5"
                @click="deleteTask(index)"
              >
                x
              </button>
            </span>
          </li>
        </ul>
      </div>
      <div class="pt-5 mt-10 border-t lg:mt-20 border-t-red-50">
        <p class="text-2xl font-semibold text-center text-white lg:text-3xl">
          Today's Completed Task
        </p>
        <ul class="mt-5">
          <li
            class="flex justify-between px-3 py-3 text-base font-semibold text-white bg-green-500 border-b lg:px-10 lg:text-xl w-80 lg:w-full x-5 border-b-gray-100 text-wrap"
            v-for="Complete in complete"
            :key="Complete"
          >
            <span>
              <p class="break-words">
                {{ Complete }}
              </p>
            </span>
          </li>
        </ul>
      </div>
    </div>
  </main>
</template>

<style scoped></style>
