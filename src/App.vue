<script setup>
  const tasks = [
  "Complete project proposal",
  "Update website content",
  "Fix bug in user authentication",
  "Prepare presentation slides",
  "Test new feature implementation",
 ];
</script>

<template>
   <div class="p-5 border border-gray-600 w-50" v-for="(task,index) in tasks">{{ index+1}}.{{ task }}</div>
</template>

<style scoped>

</style>
