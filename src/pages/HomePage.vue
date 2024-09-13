<script setup>
import { RiMenuFill } from "@remixicon/vue";
</script>

<template>
  <main class="w-screen h-full">
    <!-- hero section -->
    <section>
      <div class=" px-10 flex items-center justify-between h-10 py-8 mt-5 bg-black">
        <div class="w-1/5 text-2xl text-nowrap j font-semibold text-white">Harsh Uleedri</div>
        <div class="hidden lg:block">
          <ul
            class="flex border-t border-t-white border-opacity-50 gap-10 text-white bg-white rounded-full bg-opacity-30 backdrop-blur-sm"
          >
            <li class="px-10 py-3 hover:bg-white hover:bg-opacity-40 rounded-full text-white transition-all">Home</li>
            <li class="px-10 py-3 hover:bg-white hover:bg-opacity-40 rounded-full text-white">About</li>
            <li class="px-10 py-3 hover:bg-white hover:bg-opacity-40 rounded-full text-white">Service</li>
            <li class="px-10 py-3 hover:bg-white hover:bg-opacity-40 rounded-full text-white">Contact Us</li>
          </ul>
        </div>
        <div class="hidden w-1/5 lg:flex items-center gap-10">
          <div class="flex flex-row items-center justify-center">
            <div class="w-26 flex item-center justify-center border-t border-t-white border-opacity-50 bg-opacity-40 bg-white rounded-full transition-all">
              <input type="radio" id="button1" name="button" class="hidden peer/button1" checked>
              <label for="button1" class="px-3 py-2 text-white  peer-checked/button1:bg-white outline-none peer-checked/button1:rounded-full peer-checked/button1:bg-opacity-40">DE</label>
              <input type="radio" id="button2" name="button" class="hidden peer/button2">
              <label for="button2" class="px-3 py-2 text-white  peer-checked/button2:bg-white outline-none peer-checked/button2:rounded-full peer-checked/button2:bg-opacity-40">EN</label>
              
            </div>
          </div>
          <div>
            <button class="px-8 py-2 bg-white rounded-full font-semibold hover:bg-gray-200">login</button>
          </div>
        </div>
        <div class="lg:hidden">
          <RiMenuFill size="36px" color="white" className="my-icon"/>
        </div>
      </div>
      <div></div>
      <div></div>
    </section>
  </main>
</template>
