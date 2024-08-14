<script lang="ts" setup>
import { defineProps, computed } from "vue";

// Define props with default and not required
const props = defineProps<{
  bg: string;
  src: string;
}>();
</script>

<template>
  <div class="block lg:hover:scale-110 transition">
    <div
      class="rounded-xl w-[90px] h-[90px] flex justify-center items-center"
      :style="{ backgroundColor: props.bg }"
    >
      <img
        class="rounded-xl w-[90px] h-[90px] mx-auto my-auto"
        :src="props.src"
        alt="logo"
      />
    </div>
  </div>
</template>
