<script setup>
import backgroundImage from "../assets/background-image.jpg";
</script>

<template>
  <main class="flex grow gap-2">
    <section class="grow grid grid-cols-12 gap-2">
      <!-- First section (unchanged) -->
      <section
        class="col-span-6 flex flex-col items-center p-5 gap-10 rounded hover:bg-[#d9d9d9] hover:text-black group relative overflow-hidden"
      >
        <div class="pt-20 flex flex-col items-center justify-center">
          <p class="text-xl">The path of</p>
          <h1 class="text-3xl font-semibold">SOFTWARE ENGINEERING</h1>
        </div>
        <div
          class="flex flex-col gap-1 px-7 py-5 bg-[#1B1B1B] rounded mt-10 tracking-wide group-hover:text-white"
        >
          <h4 class="text-md">Bachelor of Technology</h4>
          <h2 class="text-lg font-bold tracking-wider">
            Computer Science and Engineering
          </h2>
          <p class="text-md opacity-75">
            Mar Baselios College of Engineering and Technology, Trivandrum
          </p>
        </div>
      </section>

      <!-- Second section with hover background -->
      <section
        class="col-span-6 flex flex-col items-center p-5 gap-10 rounded group relative overflow-hidden"
      >
        <!-- background layer -->
        <div
          class="absolute inset-0 bg-cover bg-center opacity-0 group-hover:opacity-100 transition duration-500"
          :style="{ backgroundImage: `url(${backgroundImage})` }"
        ></div>

        <!-- content layer -->
        <div
          class="pt-20 flex flex-col items-center justify-center relative z-10"
        >
          <p class="text-lg">The path of</p>
          <h1 class="text-3xl font-semibold">FITNESS TRAINING</h1>
        </div>
        <div
          class="flex flex-col gap-1 px-7 py-5 bg-[#1B1B1B] rounded mt-10 tracking-wide group-hover:text-white relative z-10"
        >
          <h4 class="text-md">Professional Diploma</h4>
          <h2 class="text-lg font-bold tracking-wider">
            Health and Fitness Training
          </h2>
          <p class="text-md opacity-75">
            CCEK NSDC, Government College, Karyavattom, Trivandrum
          </p>
        </div>
      </section>
    </section>
  </main>
</template>
