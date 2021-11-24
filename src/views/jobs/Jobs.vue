
  
<template>
  <h1>Jobs</h1>
  <div v-for="job in jobs" :key="job.id">
    <h2>{{ job.title }}</h2>
  </div>
</template>

<script>
export default {
  data() {
    return {
      jobs: [
        { title: 'Cia AEM Developer', id: 1, details: 'lorem1' },
        { title: 'Cia Web Developer', id: 2, details: 'lorem2' },
        { title: 'Cia Vue Developer', id: 3, details: 'lorem3' },
      ],
    }
  }
}
</script>

<style>
</style>