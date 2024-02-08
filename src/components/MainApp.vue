<script>

import AppComics from '../components/AppComics.vue'

export default {

  name: "MainApp",

  components:{
    AppComics,
  },

  data() {

    return {

      listComics: [
        {
          thumb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
        },
        {
          thumb:
            "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel",
        },
        {
          thumb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book",
        },
        {
          thumb:
            "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
          price: "$3.99",
          series: "Batman",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel",
        },
      ],
    };
  },
  methods: {},
};

</script>



<template>

  <main>

    
    <figure>

      <div class="jumbotron">

        <div class="btn-series">current series</div>
      </div>

    </figure>



    <div class="container-list">



      <AppComics 

      v-for="(element,index) in listComics" 
      :key="index" 
      :propsSrc="element.thumb"
      :propsSeries="element.series"
      />
      
        <!-- <figure class="list-figure">

          <img :src="element.thumb" alt="element.type">

        </figure>

        <h4>{{ element.series }}</h4> -->

      <button>load more</button>

    </div>
    

    <!-- sezione centrale azzurra -->
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
  
  background-color: #1C1C1C;

  .jumbotron{
    background-image: url(../assets/img/jumbotron.jpg);
    height: 350px;
    background-repeat: no-repeat;
    background-size: cover;
    background-position: 0% 5%;
    position: relative;

  }
  
}

.btn-series{
  position: absolute;
  padding: 15px 40px;
  font-size: 25px;
  text-transform: uppercase;
  color: white;
  font-weight: bold;
  cursor: pointer;
  background-color:#0282F9;
  bottom: - 25px;
  left: 270px;

}


.container-list{
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    row-gap: 50px;
    width: 70%;
    margin: 0 auto;
    color: white;
    background-color: #1C1C1C;
    padding-block: 50px;

    button{
      margin: 0 auto;
      border: none;
      background: none;
      background-color:#0282F9;
      padding: 15px 60px;
      font-size: 20px;
      text-transform: uppercase;
      color: white;
      font-weight: bold;
      cursor: pointer;
    }
    
  .list{
    width: calc((100% / 6) - 20px);
    text-transform: uppercase;
    // .list-figure{
    //   aspect-ratio: 1;
    //   overflow: hidden;
    //   margin-bottom: 10px;

    //   img{
    //   width: 100%;
      
    //   }
    
    // }
  
    
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
