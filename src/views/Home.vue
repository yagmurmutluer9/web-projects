<template>
  <div class="container">
    <div class="info">
      <Information />
    </div>

    <div class="projects">
      <Projects />
    </div>
  </div>
</template>

<script>
import Information from "../components/Information.vue";
import Projects from "../components/Projects.vue";

export default {
  name: "Home",
  components: {
    Information,
    Projects,
  },
};
</script>

<style scoped>
.container {
  margin: 0 auto;
  margin-top: 5vh;
  width: 100%;
  height: 100%;
  padding: 20px;
  position: relative;
}

.info {
  margin: 0 auto;
  width: 80%;
}

.projects {
  margin-top: 10vh;
  margin: 0 auto;
  width: 80%;
}

@media (max-width: 640px) {
  .container {
    width: 100%;
  }
  
  .projects {
  width: 100%;
}

}
@media (min-width: 1024px) {
  .container {
    max-width: 64rem;
  }
}
</style>
