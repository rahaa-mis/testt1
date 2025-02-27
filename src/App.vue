<template>
  <div class="manrope-font">
    <Sidebar/>
    <TheChat/>
  </div>
</template>
  

<script setup>
  import Sidebar from './components/Sidebar.vue';
  import TheChat from './components/Thechat.vue';
</script>


<style>
@import url('https://fonts.googleapis.com/css2?family=Manrope:wght@200..800&display=swap');

.manrope-font{
  font-family: "Manrope", serif;
  font-optical-sizing: auto;
  font-weight: 600;
  font-style: normal;
}
</style>
  