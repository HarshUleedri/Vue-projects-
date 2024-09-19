<script setup>
import {
  RiMenuFill,
  RiCalculatorLine,
  RiSearch2Line,
  RiStarSFill,
  RiArrowLeftLine,
  RiArrowRightLine,
  RiFacebookBoxFill,
  RiInstagramFill,
  RiYoutubeFill
} from '@remixicon/vue'
</script>

<template>
  <main class="w-screen h-full px-2 pt-2 bg-gray-200 lg:w-full">
    <!-- hero section -->
    <section
      class="rounded-3xl relative bg-cover w-full pt-10 bg-center h-[90vh] lg:h-[100vh] bg-[url('https://images.pexels.com/photos/204917/pexels-photo-204917.jpeg')] before:rounded-3xl before:absolute before:inset-0 before:bg-black/50"
    >
      <!-- navbar -->
      <div class="relative z-10 flex items-center justify-between h-10 px-5 py-8 lg:px-10">
        <div class="w-1/5 text-2xl font-semibold text-white text-nowrap j">Harsh Uleedri</div>
        <div class="hidden lg:block">
          <ul
            class="flex gap-10 text-white bg-white border-t border-opacity-50 rounded-full border-t-white bg-opacity-20 backdrop-blur-lg"
          >
            <li
              class="px-10 py-3 text-white transition-all rounded-full hover:bg-white hover:bg-opacity-40"
            >
              Home
            </li>
            <li class="px-10 py-3 text-white rounded-full hover:bg-white hover:bg-opacity-40">
              About
            </li>
            <li class="px-10 py-3 text-white rounded-full hover:bg-white hover:bg-opacity-40">
              Service
            </li>
            <li class="px-10 py-3 text-white rounded-full hover:bg-white hover:bg-opacity-40">
              Contact Us
            </li>
          </ul>
        </div>
        <div class="items-center hidden w-1/5 gap-10 lg:flex">
          <div class="flex flex-row items-center justify-center">
            <div
              class="flex justify-center transition-all bg-white border-t rounded-full backdrop-blur-lg border-opacity-40 w-26 item-center border-t-white bg-opacity-40"
            >
              <input type="radio" id="button1" name="button" class="hidden peer/button1" checked />
              <label
                for="button1"
                class="px-3 py-2 text-white outline-none peer-checked/button1:bg-white peer-checked/button1:rounded-full peer-checked/button1:bg-opacity-40"
                >DE</label
              >
              <input type="radio" id="button2" name="button" class="hidden peer/button2" />
              <label
                for="button2"
                class="px-3 py-2 text-white outline-none peer-checked/button2:bg-white peer-checked/button2:rounded-full peer-checked/button2:bg-opacity-40"
                >EN</label
              >
            </div>
          </div>
          <div>
            <button class="px-8 py-2 font-semibold bg-white rounded-full hover:bg-gray-200">
              login
            </button>
          </div>
        </div>
        <div class="px-6 py-1 bg-white rounded-full lg:hidden bg-opacity-20 backdrop-blur-lg">
          <RiMenuFill size="36px" color="white" className="my-icon" />
        </div>
      </div>
      <!-- CTA -->
      <div class="relative z-10 mt-32 lg:mt-20">
        <h1
          class="w-11/12 mx-auto text-3xl font-semibold leading-tight tracking-normal text-center text-white lg:w-1/2 lg:text-6xl lg:font-medium text-wrap"
        >
          Extraordinary nature and
          <span class="">Culture Charm</span>
        </h1>
        <p class="mt-5 text-base text-center text-white lg:text-lg">
          Exploring India is an unforgottable adventure
        </p>
      </div>
      <div>
        <div
          class="flex justify-center w-1/2 py-2 mx-auto mt-10 bg-white rounded-full lg:px-5 lg:justify-between bg-opacity-30 backdrop-blur-lg"
        >
          <div class="items-center hidden gap-10 lg:flex">
            <div class="flex items-center">
              <label for="dropdown" class="flex gap-3 text-white text-normal">
                <RiCalculatorLine size="24px" color="white" classname="my-icon" /> Date</label
              >
              <select
                id="dropdown"
                class="w-1 px-4 py-2 pr-10 mt-1 text-white bg-transparent decoration-none focus:outline-none"
              >
                <option value="option" disabled selected hidden></option>
              </select>
            </div>
            <div class="flex items-center px-8 border-white border-opacity-60 border-x">
              <label for="dropdown" class="flex gap-3 text-white text-normal">
                <RiCalculatorLine size="24px" color="white" classname="my-icon" /> Date</label
              >
              <select
                id="dropdown"
                class="w-1 px-4 py-2 pr-10 mt-1 text-white bg-transparent decoration-none focus:outline-none"
              >
                <option value="option" disabled selected hidden></option>
              </select>
            </div>
            <div class="flex items-center">
              <label for="dropdown" class="flex gap-3 text-white text-normal">
                <RiCalculatorLine size="24px" color="white" classname="my-icon" /> Date</label
              >
              <select
                id="dropdown"
                class="w-1 px-4 py-2 pr-10 mt-1 text-white bg-transparent decoration-none focus:outline-none"
              >
                <option value="option" disabled selected hidden></option>
              </select>
            </div>
          </div>
          <div>
            <button class="px-8 py-2 font-semibold bg-white rounded-full hover:bg-gray-200">
              Search
            </button>
          </div>
        </div>
      </div>
      <!-- counter meter -->
      <div
        class="absolute flex items-center justify-center w-full gap-8 pb-16 overflow-x-hidden transform -translate-x-1/2 left-1/2 -bottom-28"
      >
        <div
          class="inline-block px-20 py-3 bg-white rounded-md shadow-2xl shadow-slate-300 shadow-opacity-50"
        >
          <h2 class="text-3xl font-semibold tracking-tighter text-center text-black">10M+</h2>
          <p class="mt-1 text-sm text-center text-gray-400">Total Costomer</p>
        </div>
        <div
          class="inline-block px-20 py-3 bg-white rounded-md shadow-2xl shadow-slate-300 shadow-opacity-50"
        >
          <h2 class="text-3xl font-semibold tracking-tighter text-center text-black">10M+</h2>
          <p class="mt-1 text-sm text-center text-gray-400">Total Costomer</p>
        </div>
        <div
          class="inline-block px-20 py-3 bg-white rounded-md shadow-2xl shadow-slate-300 shadow-opacity-50"
        >
          <h2 class="text-3xl font-semibold tracking-tighter text-center text-black">10M+</h2>
          <p class="mt-1 text-sm text-center text-gray-400">Total Costomer</p>
        </div>
        <div
          class="inline-block px-20 py-3 bg-white rounded-md shadow-2xl shadow-slate-300 shadow-opacity-50"
        >
          <h2 class="text-3xl font-semibold tracking-tighter text-center text-black">10M+</h2>
          <p class="mt-1 text-sm text-center text-gray-400">Total Costomer</p>
        </div>
      </div>
    </section>
    <!-- second section -->
    <section class="px-5 mx-auto lg:px-10">
      <div class="mt-32">
        <div>
          <div>
            <h3 class="text-sm text-left text-gray-400 lg:text-lg">Best Location</h3>
          </div>
          <div class="flex flex-col justify-between mt-3 lg:items-center lg:flex-row">
            <div class="text-2xl font-semibold text-left text-black lg:w-3/4 text-wrap lg:text-7xl">
              India Tourism
            </div>
            <div class="text-base text-left text-gray-400 lg:h-2/5 lg:text-xl text-wrap">
              Extraordinary natural beauty, enjoy the rich culture, and experience the friendliness
              of the local people.
            </div>
          </div>
        </div>
      </div>
      <div class="flex flex-col gap-5 mt-10 lg:flex-row">
        <div
          class="shadow-2xl relative h-96 lg:w-3/5 rounded-2xl bg-center bg-cover bg-no-repeat bg-[url(https://images.pexels.com/photos/8112535/pexels-photo-8112535.jpeg)] before:rounded-2xl before:absolute before:inset-0 before:bg-black/50"
        >
          <div class="absolute z-10 bottom-5 left-6">
            <p class="text-3xl font-normal text-white lg:text-5xl">Uttarpradesh</p>
            <p class="text-xl font-thin text-white lg:text-4xl">India</p>
          </div>
        </div>
        <div
          class="shadow-2xl relative h-96 lg:w-2/5 bg-center rounded-2xl bg-cover bg-[url(https://images.pexels.com/photos/7104962/pexels-photo-7104962.jpeg)] before:rounded-2xl before:absolute before:inset-0 before:bg-black/50"
        >
          <div class="absolute z-10 bottom-5 left-6">
            <p class="text-3xl font-normal text-white lg:text-5xl">Kashi</p>
            <p class="text-xl font-thin text-white lg:text-4xl">India</p>
          </div>
        </div>
      </div>
      <div class="flex flex-col gap-5 mt-5 lg:flex-row-reverse">
        <div
          class="shadow-2xl relative h-96 lg:w-3/5 rounded-2xl bg-center bg-cover bg-no-repeat bg-[url(https://images.pexels.com/photos/8112535/pexels-photo-8112535.jpeg)] before:rounded-2xl before:absolute before:inset-0 before:bg-black/50"
        >
          <div class="absolute z-10 bottom-5 left-6">
            <p class="text-3xl font-normal text-white lg:text-5xl">Uttarpradesh</p>
            <p class="text-xl font-thin text-white lg:text-4xl">India</p>
          </div>
        </div>
        <div
          class="shadow-2xl relative h-96 lg:w-2/5 bg-center rounded-2xl bg-cover bg-[url(https://images.pexels.com/photos/7104962/pexels-photo-7104962.jpeg)] before:rounded-2xl before:absolute before:inset-0 before:bg-black/50"
        >
          <div class="absolute z-10 bottom-5 left-6">
            <p class="text-3xl font-normal text-white lg:text-5xl">Kashi</p>
            <p class="text-xl font-thin text-white lg:text-4xl">India</p>
          </div>
        </div>
      </div>
    </section>
    <!-- third info section -->
    <section>
      <div
        class="flex flex-col justify-center gap-20 px-5 mt-32 lg:mt-48 lg:px-10 lg:flex-row lg:gap-44"
      >
        <div
          class="relative rounded-xl w-full h-[500px] lg:h-auto px-4 lg:w-2/5 bg-cover bg-center bg-[url('https://images.pexels.com/photos/1583244/pexels-photo-1583244.jpeg')] before:rounded-2xl before:absolute before:inset-0 before:bg-black/50"
        >
          <div
            class="absolute flex justify-center px-10 py-2 mx-auto mt-10 bg-white rounded-full w-fit lg:w-11/12 bottom-36 lg:bottom-24 lg:px-5 lg:gap-10 bg-opacity-5 backdrop-blur-md"
          >
            <div class="items-center hidden gap-3 lg:flex">
              <div class="flex items-center">
                <label for="dropdown" class="flex gap-2 text-xs font-semibold text-white">
                  <RiCalculatorLine size="18px" color="white" classname="my-icon" /> Date</label
                >
                <select
                  id="dropdown"
                  class="w-1 px-2 py-2 pr-8 mt-1 text-white bg-transparent decoration-none focus:outline-none"
                >
                  <option value="option" disabled selected hidden></option>
                </select>
              </div>
              <div class="flex items-center px-5 border-white border-opacity-60 border-x">
                <label for="dropdown" class="flex gap-2 text-xs font-semibold text-white">
                  <RiCalculatorLine size="18px" color="white" classname="my-icon" /> Date</label
                >
                <select
                  id="dropdown"
                  class="w-1 px-2 py-2 pr-8 mt-1 text-white bg-transparent decoration-none focus:outline-none"
                >
                  <option value="option" disabled selected hidden></option>
                </select>
              </div>
              <div class="flex items-center">
                <label for="dropdown" class="flex gap-2 text-xs font-semibold text-white">
                  <RiCalculatorLine size="18px" color="white" classname="my-icon" /> Date</label
                >
                <select
                  id="dropdown"
                  class="w-1 px-2 py-2 pr-8 mt-1 text-white bg-transparent decoration-none focus:outline-none"
                >
                  <option value="option" disabled selected hidden></option>
                </select>
              </div>
            </div>
            <div>
              <button class="px-8 py-2 font-semibold bg-white rounded-full hover:bg-gray-200">
                Search
              </button>
            </div>
          </div>
          <div>
            <p class="absolute text-white bottom-5 lg:bottom-10">
              Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nostrum libero delectus,
              beatae atque fugiat optio nobis molestias ad. Quis, distinctio.
            </p>
          </div>
        </div>
        <div class="lg:w-1/2">
          <div>
            <p class="text-sm text-left text-gray-400 lg:text-lg">How it works</p>
            <h2 class="mt-2 text-2xl font-semibold text-left text-black text-wrap lg:text-7xl">
              One click for You
            </h2>
          </div>
          <div>
            <div
              class="flex w-full gap-5 px-5 py-5 mt-8 rounded-lg lg:mt-12 lg:w-4/5 hover:bg-white"
            >
              <div class="px-2 py-2 bg-gray-100 rounded-lg h-fit">
                <RiSearch2Line size="28px" color="black" />
              </div>
              <div>
                <div>
                  <h3 class="text-xl font-bold lg:text-2xl">Find your destination</h3>
                  <p class="text-sm text-gray-400 lg:text-base">
                    Lorem, ipsum dolor sit amet consectetur adipisicing elit. Modi delectus
                    voluptatum unde explicabo.
                  </p>
                </div>
                <div></div>
              </div>
            </div>
          </div>
          <div>
            <div class="flex w-full gap-5 px-5 py-5 mt-5 rounded-lg lg:w-4/5 hover:bg-white">
              <div class="px-2 py-2 bg-gray-100 rounded-lg h-fit">
                <RiSearch2Line size="28px" color="black" />
              </div>
              <div>
                <div>
                  <h3 class="text-xl font-bold lg:text-2xl">Find your destination</h3>
                  <p class="text-sm text-gray-400 lg:text-base">
                    Lorem, ipsum dolor sit amet consectetur adipisicing elit. Modi delectus
                    voluptatum unde explicabo.
                  </p>
                </div>
                <div></div>
              </div>
            </div>
          </div>
          <div>
            <div class="flex w-full gap-5 px-5 py-5 mt-5 rounded-lg lg:w-4/5 hover:bg-white">
              <div class="px-2 py-2 bg-gray-100 rounded-lg h-fit">
                <RiSearch2Line size="28px" color="black" />
              </div>
              <div>
                <div>
                  <h3 class="text-xl font-bold lg:text-2xl">Find your destination</h3>
                  <p class="text-sm text-gray-400 lg:text-base">
                    Lorem, ipsum dolor sit amet consectetur adipisicing elit. Modi delectus
                    voluptatum unde explicabo.
                  </p>
                </div>
                <div></div>
              </div>
            </div>
          </div>
          <div>
            <div class="flex w-full gap-5 px-5 py-5 mt-5 rounded-lg lg:w-4/5 hover:bg-white">
              <div class="px-2 py-2 bg-gray-100 rounded-lg h-fit">
                <RiSearch2Line size="28px" color="black" />
              </div>
              <div>
                <div>
                  <h3 class="text-xl font-bold lg:text-2xl">Find your destination</h3>
                  <p class="text-sm text-gray-400 lg:text-base">
                    Lorem, ipsum dolor sit amet consectetur adipisicing elit. Modi delectus
                    voluptatum unde explicabo.
                  </p>
                </div>
                <div></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- fourth section -->
    <section class="px-5 mt-20 lg:mt-32 lg:px-10">
      <div>
        <div class>
          <div>
            <h3 class="text-sm text-left text-gray-400 lg:text-lg">Tour Packages</h3>
          </div>
          <div class="flex flex-col justify-between mt-3 lg:items-center lg:flex-row">
            <div class="text-2xl font-semibold text-left text-black lg:w-3/4 text-wrap lg:text-7xl">
              Our Tourist destination
            </div>
            <div class="text-base text-gray-400 lg:w-2/5 text-wrap lg:text-xl">
              Our tourist destination offers an unrivaled blend of Natural beauty and cultural
              richness people.
            </div>
          </div>
        </div>
      </div>
      <div>
        <div class="flex flex-col mt-20 space-y-10 lg:space-y-0 lg:space-x-10 lg:flex-row">
          <div
            class="relative lg:w-1/3 w-full px-5 py-5 shadow-2xl rounded-2xl h-[600px] bg-cover bg-center bg-[url('https://images.pexels.com/photos/6827267/pexels-photo-6827267.jpeg')]"
          >
            <div class="flex justify-between">
              <div
                class="px-6 py-1 text-sm font-semibold text-white bg-white rounded-full backdrop-blur-lg bg-opacity-20 h-fit"
              >
                7 Days
              </div>
              <div
                class="flex gap-2 px-4 py-1 text-sm font-semibold text-white bg-white rounded-full h-fit bg-opacity-20 backdrop-blur-lg"
              >
                <RiStarSFill size="20px" color="yellow" /> 4.9
              </div>
            </div>

            <div
              class="absolute px-5 py-3 transform -translate-x-1/2 bg-white rounded-lg w-80 lg:w-96 left-1/2 bottom-10 bg-opacity-20 backdrop-blur-lg"
            >
              <div class="text-base text-white lg:text-lg font-extralight">
                23-August TO 29-August
              </div>
              <div class="flex items-center justify-between mt-4">
                <div class="text-xl font-semibold text-white lg:text-2xl">Indian Tour Package</div>
                <div class="text-xl font-semibold text-white lg:text-2xl">$300</div>
              </div>
            </div>
          </div>
          <div
            class="relative lg:w-1/3 w-full px-5 py-5 shadow-2xl rounded-2xl h-[600px] bg-cover bg-center bg-[url('https://images.pexels.com/photos/6827267/pexels-photo-6827267.jpeg')]"
          >
            <div class="flex justify-between">
              <div
                class="px-6 py-1 text-sm font-semibold text-white bg-white rounded-full backdrop-blur-lg bg-opacity-20 h-fit"
              >
                7 Days
              </div>
              <div
                class="flex gap-2 px-4 py-1 text-sm font-semibold text-white bg-white rounded-full h-fit bg-opacity-20 backdrop-blur-lg"
              >
                <RiStarSFill size="20px" color="yellow" /> 4.9
              </div>
            </div>

            <div
              class="absolute px-5 py-3 transform -translate-x-1/2 bg-white rounded-lg w-80 lg:w-96 left-1/2 bottom-10 bg-opacity-20 backdrop-blur-lg"
            >
              <div class="text-base text-white lg:text-lg font-extralight">
                23-August TO 29-August
              </div>
              <div class="flex items-center justify-between mt-5">
                <div class="text-xl font-semibold text-white lg:text-2xl">Indian Tour Package</div>
                <div class="text-xl font-semibold text-white lg:text-2xl">$300</div>
              </div>
            </div>
          </div>
          <div
            class="relative lg:w-1/3 w-full px-5 py-5 shadow-2xl rounded-2xl h-[600px] bg-cover bg-center bg-[url('https://images.pexels.com/photos/6827267/pexels-photo-6827267.jpeg')]"
          >
            <div class="flex justify-between">
              <div
                class="px-6 py-1 text-sm font-semibold text-white bg-white rounded-full backdrop-blur-lg bg-opacity-20 h-fit"
              >
                7 Days
              </div>
              <div
                class="flex gap-2 px-4 py-1 text-sm font-semibold text-white bg-white rounded-full h-fit bg-opacity-20 backdrop-blur-lg"
              >
                <RiStarSFill size="20px" color="yellow" /> 4.9
              </div>
            </div>

            <div
              class="absolute px-5 py-3 transform -translate-x-1/2 bg-white rounded-lg w-80 lg:w-96 left-1/2 bottom-10 bg-opacity-20 backdrop-blur-lg"
            >
              <div class="text-base text-white lg:text-lg font-extralight">
                23-August TO 29-August
              </div>
              <div class="flex items-center justify-between mt-4">
                <div class="text-xl font-semibold text-white lg:text-2xl">Indian Tour Package</div>
                <div class="text-xl font-semibold text-white lg:text-2xl">$300</div>
              </div>
            </div>
          </div>
        </div>
        <div class="flex items-center justify-center mt-16 lg:mt-20">
          <button
            class="px-10 py-2 font-semibold text-white bg-black rounded-full hover:bg-white hover:text-black"
          >
            View More
          </button>
        </div>
      </div>
    </section>
    <!-- fifth section -->
    <section class="px-5 mt-20 lg:mt-32 lg:px-20">
      <div class="flex flex-col lg:flex-row">
        <div class="flex flex-col w-full gap-10 lg:gap-20 lg:w-2/5">
          <div class="flex items-center gap-5">
            <img
              class="rounded-full size-20"
              src="https://images.pexels.com/photos/633432/pexels-photo-633432.jpeg"
              alt="profile Image"
            />
            <div class="flex flex-col gap-2">
              <p class="text-2xl font-bold text-black">harsh Uleedri</p>
              <p class="text-base text-gray-400">growing developer</p>
            </div>
          </div>
          <div class="flex justify-between lg:justify-start lg:gap-20">
            <div class="">
              <RiArrowLeftLine color="white" size="36px" />
            </div>
            <div>
              <RiArrowRightLine color="black" size="36px" />
            </div>
          </div>
        </div>
        <div class="w-full mt-10 lg:w-3/5 lg:mt-0">
          <div>
            <p class="text-lg font-medium text-center text-black text-wrap lg:text-left">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Nisi quos doloremque
              similique omnis ea quas exercitationem, error perferendis optio voluptate voluptatem
              voluptatum laboriosam laudantium assumenda fugiat veritatis obcaecati officiis quasi
              beatae. Fugit animi similique quis nostrum qui obcaecati ullam autem? Ullam magni
              molestiae quae exercitationem facilis, tempora pariatur fuga ipsa?
            </p>
          </div>
        </div>
      </div>
    </section>
    <!--sixth Section -->
    <section class="px-5 pb-32 mt-20 lg:mt-32 lg:px-20">
      <div class="flex flex-col items-center justify-center gap-5">
        <p class="text-lg text-gray-500">Our Blogs</p>
        <h2 class="text-6xl font-semibold text-center text-black">Our Travel Memories</h2>
      </div>
      <div class="flex flex-col gap-2 lg:gap-20 lg:flex-row">
        <div class="w-full h-full mt-20 overflow-hidden bg-white shadow-2xl rounded-2xl lg:w-1/2">
          <img
            class="w-full h-72 lg:h-96 rounded-2xl"
            src="https://images.pexels.com/photos/574313/pexels-photo-574313.jpeg"
            alt=""
          />
          <div class="px-5 pb-8 mt-5">
            <p class="text-sm font-normal text-gray-500">NOV 14, 2024</p>
            <h3 class="mt-5 text-2xl font-semibold text-black lg:text-3xl text-wrap">
              2024 Travel Trends - What You Need to Know
            </h3>
            <p class="mt-3 text-base font-normal text-gray-500">
              Lorem, ipsum dolor sit amet consectetur adipisicing elit. Esse, quas. Officiis ipsa
              exercitationem perspiciatis quam.
            </p>
          </div>
        </div>

        <div class="w-full mt-20 overflow-hidden bg-white shadow-2xl rounded-2xl lg:w-1/2 h-fit">
          <img
            class="w-full h-72 lg:h-96 rounded-2xl"
            src="https://images.pexels.com/photos/574313/pexels-photo-574313.jpeg"
            alt=""
          />
          <div class="px-5 pb-8 mt-5">
            <p class="text-sm font-normal text-gray-500">NOV 14, 2024</p>
            <h3 class="mt-5 text-2xl font-semibold text-black lg:text-3xl text-wrap">
              2024 Travel Trends - What You Need to Know
            </h3>
            <p class="mt-3 text-base font-normal text-gray-500">
              Lorem, ipsum dolor sit amet consectetur adipisicing elit. Esse, quas. Officiis ipsa
              exercitationem perspicitis quam.
            </p>
          </div>
        </div>
      </div>
      <div class="flex items-center justify-center mt-16 lg:mt-20">
        <button
          class="py-2 font-semibold text-white bg-black rounded-full px-14 hover:bg-white hover:text-black"
        >
          View More
        </button>
      </div>
    </section>
  </main>
  <footer class="bg-neutral-900">
    <div class="flex flex-col justify-between px-10 pt-24 pb-20 lg:px-20 lg:pt-32 lg:flex-row">
      <div
        class="flex flex-col justify-between w-full gap-20 lg:gap-0 lg:flex-row lg:px-20 lg:w-2/4"
      >
        <div>
          <p class="text-xl font-semibold text-center text-white">About</p>
          <div class="flex flex-col gap-10 mt-5">
            <p class="text-lg font-thin text-center text-slate-300">About Us</p>
            <p class="text-lg font-thin text-center text-slate-300">blogs</p>
            <p class="text-lg font-thin text-center text-slate-300">Services</p>
            <p class="text-lg font-thin text-center text-slate-300">Career</p>
          </div>
        </div>
        <div>
          <p class="text-xl font-semibold text-center text-white">About</p>
          <div class="flex flex-col gap-10 mt-5">
            <p class="text-lg font-thin text-center text-slate-300">About Us</p>
            <p class="text-lg font-thin text-center text-slate-300">blogs</p>
            <p class="text-lg font-thin text-center text-slate-300">Services</p>
            <p class="text-lg font-thin text-center text-slate-300">Career</p>
          </div>
        </div>
        <div>
          <p class="text-xl font-semibold text-center text-white">About</p>
          <div class="flex flex-col gap-10 mt-5">
            <p class="text-lg font-thin text-center text-slate-300">About Us</p>
            <p class="text-lg font-thin text-center text-slate-300">blogs</p>
            <p class="text-lg font-thin text-center text-slate-300">Services</p>
            <p class="text-lg font-thin text-center text-slate-300">Career</p>
          </div>
        </div>
      </div>
      <div class="flex flex-col w-full gap-6 mt-20 lg:mt-0 lg:w-1/3">
        <p class="text-2xl font-semibold leading-3 tracking-wider text-white">Newsletter</p>
        <p class="font-thin text-white">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Modi voluptas tempore molestias
          quasi, qui dolorum quam eos vero autem soluta?
        </p>
        <div class="flex justify-between px-4 py-2 border border-white rounded-full">
          <input
            class="px-3 text-white placeholder-white bg-transparent border-none lg:pl-5 placeholder:text-sm placeholder:font-thin focus:outline-none focus-visible:outline-none"
            type="text"
            placeholder="Enter your Email"
          />
          <button class="px-4 py-1 bg-white rounded-full lg:px-8">Search</button>
        </div>
        <div class="flex justify-start gap-3 mt-5 lg:justify-end">
          <RiFacebookBoxFill class="px-2 py-2 bg-gray-500 rounded-full" size="46px" color="white" />
          <RiInstagramFill class="px-2 py-2 bg-gray-500 rounded-full" size="46px" color="white" />
          <RiYoutubeFill class="px-2 py-2 bg-gray-500 rounded-full" size="46px" color="white" />
        </div>
      </div>
    </div>
    <div class="py-5">
      <p class="text-sm font-thin text-center text-white">
        ©️2024 Source is unreachable ( Harsh Uleedri )
      </p>
    </div>
  </footer>
</template>
