<script setup>
import { ref, onMounted } from "vue";
import Hardy from "../assets/hardy.png";
</script>

<template>
  <main class="flex grow">
    <div class="grid grid-cols-12 grid-rows-1 w-full">
      <div class="col-span-6 flex flex-col gap-15">
        <div class="grow hero-title flex flex-col justify-end">
          <h1
            class="text-8xl tracking-wider"
            style="font-family: 'Nothing You Could Do', cursive"
          >
            TOM HARDY
          </h1>
          <div
            class="mt-2 hero-subtitle"
            style="letter-spacing: 11px; font-size: 18px"
          >
            <button
              class="hover:bg-white p-1 hover:text-black hover:font-extrabold cursor-pointer button1 duration-200 ease-in"
            >
              Frontend Developer
            </button>
            &
            <button
              class="hover:bg-white p-1 hover:text-black hover:font-extrabold cursor-pointer button2 duration-200 ease-in"
            >
              Fitness Trainer
            </button>
          </div>
        </div>
        <div class="">
          <p
            class="mb-40 opacity-75 hero-description"
            style="letter-spacing: 3px; font-size: 18px; line-height: 40px"
          >
            Here’s where my dual lives collide, weaving a story of ambition,
            grit, and the relentless pursuit of what lies beyond the code and
            the iron.
          </p>
        </div>
      </div>

      <div class="col-span-6 grid grid-cols-12 overflow-hidden relative hero">
        <div
          class="absolute rounded-full w-[800px] h-[800px] bg-white left-36 top-40 hero"
          style="clip-path: inset(0 0 22px 0)"
        />
        <div class="absolute w-full h-full left-[190px] bottom-[310px]">
          <img
            :src="`${Hardy}`"
            alt="image of Tom Hardy"
            class="scale-95 mb-60"
            style="clip-path: inset(290px 0 0 0)"
          />
        </div>
      </div>
    </div>
  </main>
</template>
