<script setup>
import Header from "../ProjectComponents/Header.vue";
import Navbar from "../ProjectComponents/Navbar.vue";
</script>
<template>
  <section
    class="flex flex-col items-center justify-center bg-black text-white font-[montserrat]"
  >
    <div class="flex flex-col w-[1520px] min-h-screen rounded-lg">
      <Header />
      <Navbar />
      <slot></slot>
    </div>
  </section>
</template>
