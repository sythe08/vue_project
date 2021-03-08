<template>
  <div class="flex items-center justify-between p-5 bg-gray-700 text-gray-300 w-full flex-row flex h-16 border-b border-gray-600">
   <!-- LEFT SIDE -->
   <div class="text-red-400 font-bold uppercase">Animex</div>
   <!-- MIDDLE -->
   <ul class="flex items-center flex-wrap justify-evenly ml-16 w-1/2 hidden md:flex">
     <li class="flex flex-row items-center"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6"></path></svg><a href="/">Home</a></li>
     <li class="flex flex-row items-center"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.75 17L9 20l-1 1h8l-1-1-.75-3M3 13h18M5 17h14a2 2 0 002-2V5a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path></svg><a href="/">Watch</a></li>
     <li class="flex flex-row items-center"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14.828 14.828a4 4 0 01-5.656 0M9 10h.01M15 10h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path></svg><a href="/">About</a></li>
   </ul>
   <!-- RIGHTT SIDE -->
   <div class="flex flex-row items-center justify-evenly px-6 py-3 w-1/2 md:w-1/4">
     <input placeholder="Search..." type="input" value="" class="text-black-800 w-full font-light mr-2 outline-none bg-transparent" />
    <button><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"></path></svg></button>
   </div>
  </div>
</template>

<script>
  export default {
    name:'NavBar'
  }
</script>

<style>
</style>