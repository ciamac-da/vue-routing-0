  <template>
  <h1>Jobs</h1>
  <div v-for="job in jobs" :key="job.id" class="job">
  <router-link :to='{ name: "JobDetails", params: { id: job.id }}'>
    <h2>{{ job.title }}</h2>
  </router-link>
  </div>
</template>

<script>
export default {
  data() {
    return {
      jobs: [
        { title: 'Cia AEM Developer', id: 1, details: 'lorem1' },
        { title: 'Cia MERN-STACK Developer', id: 2, details: 'lorem1' },
        { title: 'Cia Web Developer', id: 3, details: 'lorem2' },
        { title: 'Cia Vue Developer', id: 4, details: 'lorem3' },
      ],
    }
  }
}
</script>

<style>
.job h2 {
    background: "#333";
    padding: 20px;
    border-radius: 10px;
    margin: 10px auto;
    color: gray;
    cursor: pointer;
    max-width: 600px;
}
.job h2:hover {
    background: #ddd;
}
.job a {
    text-decoration: none;
}
</style>