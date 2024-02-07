<script>
// import

export default {
  name: "FooterApp",
};

</script>



<template>

  <footer>

    <section class="footer-section">

      <div class="list-container">


        <div>
  
          <h1>dc comics</h1>
          <ul>
            <li><a href="">characters</a></li>
            <li><a href="">comics</a></li>
            <li><a href="">movies</a></li>
            <li><a href="">TV</a></li>
            <li><a href="">games</a></li>
            <li><a href="">video</a></li>
            <li><a href="">news</a></li>
          </ul>
  
          <h1>shop</h1>
          <ul>
            <li><a href="">shop DC</a></li>
            <li><a href="">shop DC collection</a></li>
          </ul>
  
        </div>
  
        <div>
  
          <h1>dc</h1>
          <ul>
            <li><a href="">terms of use</a></li>
            <li><a href="">privacy pilicy (new)</a></li>
            <li><a href="">ad choices</a></li>
            <li><a href="">advertising</a></li>
            <li><a href="">jobs</a></li>
            <li><a href="">subscription</a></li>
            <li><a href="">talent workshops</a></li>
            <li><a href="">CPSC certificates</a></li>
            <li><a href="">rating</a></li>
            <li><a href="">shop help</a></li>
            <li><a href="">contact us</a></li>
            </ul>
  
          </div>
  
          <div>
  
            <h1>sites</h1>
            <ul>
              <li><a href="">DC</a></li>
              <li><a href="">MAD magazine</a></li>
              <li><a href="">DC kids</a></li>
              <li><a href="">DC universe</a></li>
              <li><a href="">DC power visa</a></li>
            </ul>
  
          </div>
          
      </div>
      
      <figure>

        <img src="../assets/img/dc-logo-bg.png" alt="">

      </figure>


    </section>


    <div class="sign-up-bar">

      <section class="sign-up-bar-section">

        <button>sign-up now!</button>

        <div>
          
          <ul class="logo-list">
            <li><a class="follow" href="">follow</a></li>
            <li>
              <a href="">
                <img src="../assets/img/footer-facebook.png" alt="">
              </a>
            </li>
            <li>
              <a href="">
                <img src="../assets/img/footer-twitter.png" alt="">
              </a>
            </li>
            <li>
              <a href="">
                <img src="../assets/img/footer-youtube.png" alt="">
              </a>
            </li>
            <li>
              <a href="">
                <img src="../assets/img/footer-pinterest.png" alt="">
              </a>
            </li>
            <li>
              <a href="">
                <img src="../assets/img/footer-periscope.png" alt="">
              </a>
            </li>
          </ul>

        </div>

      </section>




    </div>

  </footer>

  
</template>



<style lang="scss" scoped>

@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

footer{
  background-image: url(../assets/img/footer-bg.jpg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
}

.footer-section{
  height: 400px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 70%;
  margin: 0 auto;
  overflow: hidden;
  
  div{
    
    h1{
      text-transform: uppercase;
      font-weight: bold;
      color: white;
      padding-block: 10px;
    }
    ul{
      list-style-type: none;
      
      li{
        line-height: 160%;

        a{
          text-decoration: none;
          color: white;
          text-transform: capitalize; 
          font-size: 13px;
          opacity: 50%;
        }
        
      }
    }
  }
}

.list-container{
  display: flex;
  gap: 30px;
}

.sign-up-bar{
  background-color: #303030;
  height: 150px;
  .sign-up-bar-section{
    width: 70%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 150px;
  }
}

button{
  border: 2px solid #0282F9;
  background: none;
  padding: 15px;
  font-size: 15px;
  text-transform: uppercase;
  color: white;
  font-weight: bold;
  cursor: pointer;
}

.logo-list{
  list-style-type: none;
  display: flex;
  align-items: center;
  gap: 20px;
  .follow{
    text-decoration: none;
    font-size: 20px;
    text-transform: uppercase;
    color: #0282F9;
    font-weight: bold;
  }
}

</style>