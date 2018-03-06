<template>
  <div id="app">
    <HeaderBar/>

    <HeroSearch/>

    <HomeContent/>

    <Footer/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import StarRating from './components/StarRating'
import HeaderBar from './components/HeaderBar'
import HeroSearch from './components/HeroSearch'
import HomeContent from './components/HomeContent'

export default {
  name: 'App',
  components: {
    HelloWorld,
    StarRating,
    HeaderBar,
    HeroSearch,
    HomeContent
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
