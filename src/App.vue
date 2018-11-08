<template>
  <div id="app">
    <!-- <nav class="navbar is-primary" role="navigation" aria-label="main navigation">
      <div class="navbar-brand">
        <router-link to='/' class ='navbar-item'>MarketPulse</router-link>
      </div>

      <div class="navbar-end">
        <router-link to='About' class ='navbar-item'>About</router-link>
      </div>
    </nav> -->

    <div class="container">
    </div>

    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style lang='scss'>
  @import 'main.scss';

  // .navbar {
  //   @include phone {
  //     padding: 40px
  //   }
  // }
</style>
