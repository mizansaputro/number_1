<script setup lang="ts"></script>

<template>
  <div class="p-4 grid grid-cols-6 gap-x-6 gap-y-4">
    <div class="card-container items-center col-span-6 xs:h-[12dvh] lg:h-fit">
      1
    </div>
    <div
      v-for="item in [2, 3]"
      class="card-container lg:col-span-3 xs:col-span-6"
    >
      {{ item }}
    </div>
    <div class="xs:col-span-6 lg:col-span-4 flex flex-col gap-4">
      <div class="card-container w-full">
        <div class="card-content w-full xs:h-[30dvh] lg:h-[15vh]">4</div>
      </div>
      <div class="grid grid-cols-3 gap-4">
        <div v-for="item in [5, 6, 7]" class="card-container col-span-1">
          {{ item }}
        </div>
      </div>
    </div>
    <div class="card-container xs:col-span-6 lg:col-span-2 items-start">
      <div class="grid grid-cols-3 gap-2 w-full">
        <div
          v-for="item in [8, 9, 10]"
          class="xs:col-span-1 lg:col-span-3 card-content"
        >
          {{ item }}
        </div>
      </div>
    </div>
  </div>
</template>
