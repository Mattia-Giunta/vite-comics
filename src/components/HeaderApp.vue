<script>
// import

export default {
  name: "HeaderApp",
};

</script>



<template>

<header>

  <nav>

    <figure>

      <img src="../assets/img/dc-logo.png" alt="logo dc">

    </figure>

    <div>

      <ul>

        <li><a href="">characters</a></li>
        <li><a href="">comics</a></li>
        <li><a href="">movies</a></li>
        <li><a href="">tv</a></li>
        <li><a href="">games</a></li>
        <li><a href="">collectibles</a></li>
        <li><a href="">video</a></li>
        <li><a href="">fans</a></li>
        <li><a href="">news</a></li>
        <li><a href="">shop</a></li>

      </ul>

    </div>

  </nav>

</header>
  
  

</template>



<style lang="scss" scoped>

@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

figure{
  padding: 10px;

  img{
    height: 80px;
  }
}



nav{
  height: 100px;
  display: flex;
  justify-content: space-between;
  align-items: center;

  ul{
    list-style-type: none;
    display: flex;
    gap: 30px;
    

    a{
      text-decoration: none;
      color: black;
      text-transform: uppercase;
      height: 100%;
      font-size: 13px;
      font-weight: bold;
      display: flex;
      height: 100px;
      align-items: center;
      

      &:hover{
        border-bottom: 5px solid #0282F9;
        color: #0282F9;
      }
    }
  }
}


</style>