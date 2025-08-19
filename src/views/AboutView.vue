<script setup>
import AboutHardy from "../assets/AboutHardy.png";
</script>
<template>
  <main class="flex grow">
    <div class="grid grid-cols-12 grid-rows-1 w-full">
      <div class="col-span-6 about-image">
        <img
          :src="`${AboutHardy}`"
          alt="Side Profile of Tom Hardy"
          class="h-full object-contain z-10"
        />
      </div>
      <div class="col-span-6 self-center">
        <div
          class="px-15 py-10 rounded-2xl flex flex-col justify-center gap-5 tracking-widest text-lg text-justify font-extralight"
        >
          <p class="about-title about-description">
            Hi, I'm
            <span class="text-2xl tracking-wider font-normal"> Roshan!</span>
          </p>
          <p class="about-description">
            Here’s where my dual lives as a
            <i class="font-normal">Frontend Software Engineer</i> and
            <i class="font-normal">Fitness Coach </i>collide, weaving a story of
            ambition, grit, and the relentless pursuit of what lies beyond the
            code and the iron.
          </p>
        </div>
      </div>
    </div>
  </main>
</template>
