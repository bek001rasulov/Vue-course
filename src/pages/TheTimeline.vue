<template>
  <div>
    <ul>
      <li
        v-for="i in [0, 1, 2, 3, 4, 5]"
        class="relative flex flex-col items-center gap-2 border-b border-gray-200 py-10 px-4"
      >
        <a
          href="#"
          class="absolute -bottom-4 rounded bg-gray-100 px-2 font-mono text-lg text-gray-500"
          >{{ i }}:00</a
        >
      </li>
    </ul>
  </div>
</template>
