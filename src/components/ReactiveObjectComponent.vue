<script setup>
   import { reactive } from 'vue'; 
   const  data = reactive(
    {
        count: 0,
    }
   );

   function incrementValue(){
      data.count++; 
   }
</script>

<template>
        <div class="">
            <p>Count: {{ data.count }}</p><br>
            <button class="btn btn-primary text-black" type="button" @click="incrementValue()">Increment</button>
         </div>
</template>

<style scoped>

</style>