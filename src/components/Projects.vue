<template>
  <div class="projects">
    <ul class="project-list">
      <Project
        v-for="project in projects"
        :key="project.projectID"
        v-bind:project="project"
      />
    </ul>
  </div>
</template>

<script scoped>
import Project from "../components/Project.vue";
export default {
  name: "Projects",
  components: {
    Project,
  },
  data() {
    
    return {
      projects: [
        {
        projectID: 1,
        name: "Weather App",
        desc: "A web application that shows weathers and allows you to add/remove them. All the metedata is retrieved from Weather API.",
        img: "weather-app",
        link: ["https://github.com/yagmurmutluer9/weather-vue-app", "https://weather-firebase-vue.netlify.app"],
        tech: ["Vue", "Firebase"],
        },
        {
        projectID: 2,
        name: "Anime Search",
        desc: "A web application that search anime characters and allows you to filter them. All the metadata is retrieved from Anime API.",
        img: "anime-app",
        link: ["https://github.com/yagmurmutluer9/vue-anime-app", "https://vue-anime-app.netlify.app"],
        tech: ["Vue", "Anime API", "CSS"],
        },
             {
        projectID: 3,
        name: "Responsive Website",
        desc: "A responsive web application.",
        img: "responsive-website",
        link: ["https://github.com/yagmurmutluer9/responsive-website-blog", "https://responsive-website-ymutluer9.netlify.app"],
        tech: ["Javascript", "HTML5", "CSS"],
        },
        
         {
        projectID: 4,
        name: "React To-Do",
        desc: "A web application that add/remove/filter to-do's and has local storage.",
        img: "react-todo",
        link: ["https://github.com/yagmurmutluer9/todo-react-app", "https://adoring-heisenberg-8da1d5.netlify.app"],
        tech: ["React", "CSS"],
        },
        
             

      ],
    };
  },
};
</script>

<style>
.projects {
  display: flex;
  justify-content: center;
}

.project-list {
width: 100%;
display: flex;
flex-direction: column;
margin-top: 30px;
}
</style>
