<script setup>
import { computed } from "vue";
import { getIcon } from "../utils/IconSelector";

const props = defineProps({
  name: String,
  classes: {
    type: String,
    default: "",
  },
});

const svgIcon = computed(() => getIcon(props.name));
</script>
<template>
  <span v-html="svgIcon" :class="classes"></span>
</template>
