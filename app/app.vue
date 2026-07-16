<template>
  <div>

    woop!

    <pre v-if="error">{{ error }}</pre>

    <pre v-else>{{ JSON.stringify(data, null, 2) }}</pre>
  </div>
</template>


<script setup lang="ts">
console.log('joop!')
const { data, error } = await useFetch('/api/helloworld')
</script>