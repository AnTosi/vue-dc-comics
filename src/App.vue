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

      </div>
      <div class="bottom_page">

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
#section_two img {
  height: 50px;
}
@import './assets/variables.scss';
@import './assets/common.scss';
</style>
