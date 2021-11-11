<template>
  <div id="app">
    <header id="site_header" class="d-flex container align-items-center py-3">

      <Logo/>   

      <div class="nav col-60 d-flex align-items-center">
        <ul class="d-flex">
          <li>CHARACTERS</li>
          <li>COMICS</li>
          <li>MOVIES</li>
          <li>TV</li>
          <li>GAMES</li>
          <li>COLLECTIBLES</li>
          <li>VIDEOS</li>
          <li>FANS</li>
          <li>NEWS</li>
          <li>SHOP</li>
        </ul>
      </div>  
    </header>
    <main>
      <section id="section_one" class="bg_black">
        <div class="text_white py-4 font-size-2 container bg_black">
          --> Content goes here &#60;--
        </div>
      </section>

      <section id="section_two" class="d-flex justify-content-around bg_blue py-5">
          <BlueBand/>
      </section>
    </main>

    <footer id="site_footer">
      <div class="links">
        <div class="text_white container d-flex">
          <div class="links-wrapper col-33 d-flex flex-wrap flex-column">
            <div class="link-sub-area col-33 d-flex flex-wrap flex-column">
              <h3>DC COMICS</h3>
              <ul>
                <li>Characters</li>
                <li>Comics</li>
                <li>Movies</li>
                <li>TV</li>
                <li>Games</li>
                <li>Videos</li>
                <li>News</li>
              </ul>
            </div>

            <div class="link-sub-area col-33 d-flex flex-wrap flex-column">
              <h3>SHOP</h3>
              <ul>
                <li>Shop DC</li>
                <li>Shop DC Collectibles</li>
              </ul>
            </div>

            <div class="link-sub-area col-33 d-flex flex-wrap flex-column">
              <h3>DC</h3>
              <ul>
                <li>Terms Of Use</li>
                <li>Privacy policy (New)</li>
                <li>Ad Choices</li>
                <li>Advertising</li>
                <li>Jobs</li>
                <li>Subscriptions</li>
                <li>Talent Workshops</li>
                <li>CPSC Certificates</li>
                <li>Ratings</li>
                <li>Shop Help</li>
                <li>Contact Us</li>
              </ul>
            </div>

            <div class="link-sub-area col-33 d-flex flex-wrap flex-column-">
              <h3>SITES</h3>
              <ul>
                <li>DC</li>
                <li>MAD Magazine</li>
                <li>DC Kids</li>
                <li>DC Universe</li>
                <li>DC Power Visa</li>
              </ul>
            </div>

          </div>
          <div class="dc_fat_logo">
            
          </div>
        </div>
      </div>
      <div class="page_bottom bg_dark">
        <div class="container py-4 d-flex align-items-center">
          <div class="col-50 left-bottom">
            <button>SIGN-UP NOW!</button>
          </div>
          <div class="col-50 right-bottom d-flex align-items-center">
            <span class="mx-2">FOLLOW US</span>
            <img class="mx-2" src="./assets/footer-facebook.png" alt="">
            <img class="mx-2" src="./assets/footer-twitter.png" alt="">
            <img class="mx-2" src="./assets/footer-youtube.png" alt="">
            <img class="mx-2" src="./assets/footer-pinterest.png" alt="">
            <img class="mx-2" src="./assets/footer-periscope.png" alt="">
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>

import Logo from './components/Logo.vue';
import BlueBand from './components/BlueBand.vue';

export default {
  name: 'App',
  components: {
    Logo,
    BlueBand
    
  }
}
</script>

<style lang="scss">
// #app {
  //   font-family: Avenir, Helvetica, Arial, sans-serif;
//   -webkit-font-smoothing: antialiased;
//   -moz-osx-font-smoothing: grayscale;
//   text-align: center;
//   color: #2c3e50;
//   margin-top: 60px;
// }

@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600;700&display=swap');
@import './assets/variables.scss';
@import './assets/common.scss';

#section_two img {
  height: 50px;
}

.links {
  background-image: url('./assets/footer-bg.jpg');
  background-size: cover;
  height: 370px;
  flex-wrap: wrap;

  .container {
    height: 370px;
  h3 {
    font-size: 1.1rem;
    font-weight: 700;
    margin-top: 1rem;
    margin-bottom: 1rem;
  }

  li {
    list-style: none;
    padding-left: 0;
    color: $greyed;
    padding-bottom: 5px;
    font-size: 0.8rem;
    display: block;
    &:hover {
    cursor: pointer;
    }
  }

    
  .links-wrapper {
    text-align: left;
    align-items: flex-start;
    height: 370px;
    padding: 1.5rem 0 1.5rem 0;
  }
  .link-sub-area {
    height: fit-content;
    padding-right: 1rem;;
  }
}
}

.dc_fat_logo {
  // position: relative;
  width: 66%;
  // img {
  // height: 550px;
  // position: absolute;
  // right: 0;
  // top: 50%;
  // transform: translate(0, -50%);
  // }
  background-image: url('./assets/dc-logo-bg.png');
  background-repeat: no-repeat;
  background-position-x: right;
  background-position-y: 50%;
}

.page_bottom{
  height: 110px;
  button {
    border-style: none;
    background-color: $dark;
    border: 1px solid $main-blue;
    padding: 0.6rem;
    color: white;
    font-size: 0.8rem;
    
    &:hover {
    cursor: pointer;
    }
  }
  img {
    height: 40px;
  }
  .right-bottom {
    justify-content: right;
    align-items: center;
    color: $main-blue;
    font-weight: 700;
    font-size: 1rem;
  }
}

</style>
