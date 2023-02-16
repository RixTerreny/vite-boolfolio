<script>
export default{
    name:'Show',
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
            <div class="ms-2" v-for="tags in project.types">
            {{tags.type}}
            </div>
          </div>
          <a href="">Show </a>
        </li>
      </ul>
    </div>
</template>

<style>

</style>