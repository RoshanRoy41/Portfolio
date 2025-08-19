<script setup>
import { RouterLink } from "vue-router";

const navbarList = [
  { name: "Home", path: "/" },
  { name: "About", path: "/about" },
  { name: "Qualifications", path: "/qualifications" },
  { name: "Career", path: "/career" },
  { name: "Projects", path: "/projects" },
  { name: "Contact", path: "/contact" },
];
</script>
<template>
  <section class="flex min-h-20 pt-5 pb-2 px-3 bg-black text-white">
    <ul class="flex flex-1 gap-4 justify-around items-end px-32">
      <li
        v-for="navbarListItem in navbarList"
        class="hover:pb-1 hover:border-b-2 hover:border-white transition-all ease-in-out"
        :key="navbarListItem.name"
      >
        <RouterLink :to="`${navbarListItem.path}`">{{
          navbarListItem.name
        }}</RouterLink>
      </li>
    </ul>
  </section>
</template>
