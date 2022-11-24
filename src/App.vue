<script setup lang="ts">
import sidebar from "@/components/Sidebar.vue";
</script>
<template>
 <sidebar />
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
