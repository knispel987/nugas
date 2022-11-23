<template>
 <nav class="fixed w-60 h-full">
  <ul
   class="text-4xl [&>*]:capitalize focus:[&>*]:outline focus:[&>*]:outline-1 hover:[&>*]:bg-gray-200 [&>*]:p-2 [&>*]:w-full [&>*]:flex h-full text-white bg-sky-400 overflow-auto"
  >
   <router-link :to="{ name: 'multimedia' }">multimedia</router-link>
   <router-link :to="{ name: 'materi' }">materi</router-link>
   <router-link :to="{ name: 'credits' }">credits</router-link>
   <router-link :to="{ name: 'about' }">about</router-link>
  </ul>
 </nav>
 <div class="ml-60 text-xl">
  <div class="bg-white [&>*]:px-3">
   <!-- kepala -->
   <div class="p-2 place-items-center sticky top-0 bg-white shadow-2xl">
    <div class="w-full">
     <div class="flex">
      <p class="uppercase">multimedia XII-MM</p>
     </div>
    </div>
   </div>
   <!-- /kepala -->

   <!-- konten -->
   <div class="">
    <router-view />
   </div>
   <!-- /konten -->
  </div>
 </div>
</template>

<style>
nav a.router-link-exact-active {
 background-color: white;
 color: black;
}
</style>
