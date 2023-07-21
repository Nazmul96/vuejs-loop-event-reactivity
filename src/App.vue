<script setup>

  const items = [1,2,3,4,5]

</script>

<template>
    <div class="p-5 border border-gray-600 w-40" v-for="item in items">{{ item }}</div>
</template>

<style scoped>
 
</style>
