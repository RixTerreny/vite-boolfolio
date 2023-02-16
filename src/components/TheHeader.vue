<script>
export default {
  data() {
    return {
    }
  }
}
</script>

<template>
<div class="container py-2">
    <div class="row align-item-center">
        <div class="col-6 fs-3">Boolfolio</div>
        <div class="col-6 text-end fs-5">
            <a href="">Home</a>
            <a href="">Vai</a>
        </div>
    </div>
</div>
</template>

<style scoped lang="scss">
@use '../main.scss' as *;
div a{
    text-decoration: none;
    margin-left: 35px;
}

div a:hover{
    color: rgb(230, 230, 230);
}
</style>