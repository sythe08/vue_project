<template>
  <div class="bg-gray-700 text-gray-200 container-lg grid grid-cols-3 grid-rows-2 gap-4 p-6 h-full md:w-full md:grid-rows-3">
    <!-- LEFT SIDE -->
    <div class="text-center row-start-1 row-end-2 col-span-2 md:row-start-1 md:row-end-2 md:flex md:flex-col md:justify-center md:items-center">
      <h2 class="tracking-widest leading-2 mb-4 font-xl font-normal text-xl uppercase">High Quality Anime</h2>
      <p class="font-light text-sm lesding-4 tracking-widest">Animex offers high quality anime. Probably the best website to watch anime! </p>
    </div>
    <!-- RIGHT SIDE -->
    <div class="col-start-2 row-end-3 col-end-4 row-start-2 row~end-3 md:row-end-3 md:row-end-4">
      <img class="object-cover" src="../assets/preview_anime_bg.jpg" alt="Preview" />
    </div>
  </div>
</template>

<script>
  export default {
    name: 'Hero'
  }
</script>

<style>
</style>