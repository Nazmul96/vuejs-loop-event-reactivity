<script setup>
  import {countries} from './data/country';
  const name_start = "B";
  const country_find = countries.filter(
    (country) => country.country.toUpperCase().startsWith(name_start)
  )
  
</script>

<template>
      <h1>Country Name Start With {{ name_start }}</h1>
      <div>
        <p v-for="(country,index) in country_find" :key="index" style="width: 50px;text-align:center;">{{index+1}}:{{ country.country }}</p>
      </div>
</template>

<style scoped>

</style>
