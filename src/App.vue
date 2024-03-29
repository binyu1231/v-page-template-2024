<template>
  <!-- font-sans -->
  <main>
    <RouterView />
  </main>
</template>
<script setup lang="ts">
// @ts-ignore
import AOS from 'aos'


onMounted(() => {
  AOS.init({
    once: true,
    disable: 'phone',
    duration: 500,
    easing: 'ease-out-cubic',
  })

 
})


</script>