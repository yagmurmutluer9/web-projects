<template>
  <div class="container">
    <div class="title">
      <h3>{{ project.name }}</h3>
    </div>

    <div class="project-links">
      <a :href="`${project.link[0]}`" target="_blank">
        <i class="fab fa-github fa-lg link"></i>
      </a>
      <a :href="`${project.link[1]}`" target="_blank">
        <i class="fas fa-external-link-alt fa-lg link"></i>
      </a>
    </div>

    <div class="project-img">
      <img :src="require(`../assets/imgs/${project.img}.png`)" alt="" />
    </div>

    <div class="project-desc">
      <p>{{ project.desc }}</p>
    </div>

    <div class="project-tech" >
      <h3 class="tech-item" v-for="tech in project.tech" :key="tech.id" >  ·  {{ tech }} </h3>
    </div>
  </div>
</template>

<script>
export default {
  name: "Project",

  props: ["project"],
};
</script>

<style scoped>
.container {
  width: 100%;
  margin-bottom: 30px;
  padding: 40px;
  position: relative;
  justify-content: center;
}

.title {
  position: absolute;
  top: 0%;
  left: 50%;
  transform: translateX(-50%);
  padding: 0 10px;
}

.project-links {
  position: absolute;
  right: 0;
  top: 0;
  padding: 7px;
}

.link {
  margin-left: 10px;
  color: black;
}

.link:hover {
  color:blue;
}

.link:visited {
  color: rgb(39, 13, 87);
}

.project-img {
  width: 100%;
  padding: 0px 8px;
  margin-bottom: 8px;
}

.project-tech {
  margin-top: 10px;
  display: flex;
  
}

.tech-item {
  font-weight: 600;
  font-size: 16px;
  margin-right: 10px;
}


img {
  width: 100%;
}

@media (max-width: 640px) {
  .title {
    width: 100%;
  }
  
 
}
</style>
