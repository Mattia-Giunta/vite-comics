<script>
// import


export default {
  name: "AppComics",

  props:{
    propsSrc: String,
    propsSeries: String,

  }
};

</script>



<template>

<div  class="list">
    <figure class="list-figure">

    <img :src="propsSrc" alt="propsSeries">

    </figure>

    <h4>{{ propsSeries }}</h4>
</div>


</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;


.list-figure{
    aspect-ratio: 1;
    overflow: hidden;
    margin-bottom: 10px;

    img{
    width: 100%;
      
    }
    
}


</style>