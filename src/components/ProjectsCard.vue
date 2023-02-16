<script>
export default{
  props:['projects'],
}
</script>

<template>
<div class="container">
      <h3 class="mb-4">Progetti:</h3>
      <ul class="mb-4" v-for="project in projects">
        <li>{{ project.name }} 
          <div class="d-flex">
            
            <div class="ms-4">Tags:</div>
            <div class="ms-2" v-for="tag in project.types">
            {{tag.type}}
            </div>
          </div>
          <a href="">Show </a>
        </li>
      </ul>
    </div>
</template>

<style scoped lang="scss">
@use '../main.scss' as *;

</style>