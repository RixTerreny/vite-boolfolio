<script >
import axios from "axios";
import TheHeader from './components/TheHeader.vue'
import ProjectsCard from './components/ProjectsCard.vue'
export default{
  components:{TheHeader,ProjectsCard},
  data(){
    return{
      projects:[]
    };
  },
  methods:{
    fetchProjects(){
      axios.get('http://127.0.0.1:8000/api/projects')
      .then((resp)=>{
        this.projects = resp.data;
      })
    }
  },
  mounted(){
    this.fetchProjects();
  }
}
</script>

<template>
  <div class="bg-dark text-white gg">
    <TheHeader/>
    <hr>
    <ProjectsCard :projects="projects"/>
    
  </div>
</template>

<style lang="scss">
@use './main.scss' as *;
.gg{
  min-height: 100vh;
}
</style>
