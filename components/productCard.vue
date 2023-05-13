<template>
  
    <div 
      class="max-w-sm rounded overflow-hidden shadow-sm mb-4 dark:bg-gray-900"
    >
      <img
        class="w-full"
        src="https://tailwindcss.com/img/card-top.jpg"
        alt="Sunset in the mountains"
      />
      <div class="px-6 py-4 pb-2">
        <div class="font-bold text-xl mb-2 dark:text-white">
         Product:  {{ product.name }}
        </div>
        <p class="text-gray-700 dark:text-gray-300 text-base">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus
          quia, nulla! 
        </p>
      </div>
      <div class="px-6 py-4">
      
      </div>
    </div>




</template>

<script setup>
const {product} = defineProps(['product'])
console.log("beeeer",product)
</script>

<style  scoped>

</style>