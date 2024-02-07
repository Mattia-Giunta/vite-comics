<script>
// import

export default {
  name: "MainApp",
};

</script>



<template>

  <main>

    <figure>

      <div>--Contenuto--</div>

    </figure>

    <section>

      <ul>

        <li>
          <img src="../assets/img/buy-comics-digital-comics.png" alt="">
          <span>digital comics</span>
        </li>
          
        <li>
          <img src="../assets/img/buy-comics-merchandise.png" alt="">
          <span>dc merchandise</span>
        </li>
          
        <li>
          <img src="../assets/img/buy-comics-subscriptions.png" alt="">
          <span>subscription</span>
        </li>
          
        <li>
          <img class="location-img" src="../assets/img/buy-comics-shop-locator.png" alt="">
          <span>comin location</span>
        </li>
          
        <li>
          <img src="../assets/img/buy-dc-power-visa.svg" alt="">
          <span>dc power visa</span>
        </li>
          

      </ul>

    </section>


  </main>

  

</template>



<style lang="scss" scoped>

@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

figure{
  height: 150px;
  background-color: #1C1C1C;
  
  div{
    width: 70%;
    margin: 0 auto;
    height: 100%;
    color: white;
    display: flex;
    align-items: center;
    font-size: 30px;
  }
}

section{
  height: 150px;
  background-color: #0282F9;
  

  ul{
    width: 70%;
    margin: 0 auto;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-evenly;
    li{
      display: flex;
      align-items: center;
      gap: 15px;
      img{
        width: 50px;
      }
      span{
        color: white;
        text-transform: uppercase;
        font-size: 14px;
      }
    }
  }
}

.location-img{
  width: 40px;
}


</style>
