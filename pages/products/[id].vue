<template>
    <div>
  <p> products page for {{ id }}</p>
  <p> Lorem ipsum dolor sit, amet consectetur adipisicing elit. Numquam tempora magni nam sed, voluptas, dolorum sint nostrum mollitia porro necessitatibus, eaque maiores. Animi enim et repellendus nam quos totam eos?</p>
    </div>
</template>

<script setup>
const {id} = useRoute().params
definePageMeta({
    layout: 'products',
       title: 'products',
       description: 'this is the products page'
   })
</script>

<style lang="scss" scoped>

</style>