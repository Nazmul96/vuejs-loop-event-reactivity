<script setup>
 const tasks = [
  { id: 1, title: "Complete project proposal", status: "In Progress" },
  { id: 2, title: "Update website content", status: "Completed" },
  { id: 3, title: "Fix bug in user authentication", status: "In Progress" },
  { id: 4, title: "Prepare presentation slides", status: "Pending" },
  { id: 5, title: "Test new feature implementation", status: "In Progress" },
  { id: 6, title: "Test new feature", status: "Completed" },
];

function getCompleteTasks(){
  return tasks.filter(task =>'Completed'==task.status)
}
function getTasksInProgress(){
  return tasks.filter(task =>'In Progress'==task.status)
}
function getPendingInProgress(){
  return tasks.filter(task =>'Pending'==task.status)
}
</script>

<template>
   <h2>Completed Task</h2>
   <div class="p-5 border border-gray-600 text-left" v-for="(task,index) in getCompleteTasks()" :key="index">{{ index+1 }}.{{ task.title }}</div>

   <h2>In Progress Task</h2>
   <div class="p-5 border border-gray-600 text-left" v-for="(task,index) in getTasksInProgress()" :key="index">{{ index+1 }}.{{ task.title }}</div>

   <h2>Pending Task</h2>
   <div class="p-5 border border-gray-600 text-left" v-for="(task,index) in getPendingInProgress()" :key="index">{{ index+1 }}.{{ task.title }}</div>
</template>

<style scoped>

</style>
