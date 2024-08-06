<script setup>
import { generateTimelineItems } from "../functions.js";

const timelineItems = generateTimelineItems();
</script>

<template>
  <div class="mt-[80px]">
    <ul>
      <li
        v-for="{ hour } in timelineItems"
        class="relative flex flex-col items-center gap-2 border-t border-gray-200 py-10 px-4"
        :key="hour"
      >
        <a
          href="#"
          class="absolute -top-4 rounded bg-gray-100 px-2 font-mono text-lg text-gray-500"
          >{{ hour }}:00</a
        >
      </li>
    </ul>
  </div>
</template>
