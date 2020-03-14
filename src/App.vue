<template>
  <div id="app">
     <myheader/>
     <compobody msg = "When anxious, uneasy and bad thoughts come, I go to the sea, and the sea drowns them out with its great wide sounds, 
     cleanses me with its noise, and imposes a rhythm upon everything in me that is bewildered and confused." content = "All you need is a good dose of vitamin sea. :)" votes = '0'/>
     
     <myfooter/>
  </div>
</template>

<script>
import myheader from './components/myheader.vue'
import compobody from './components/compobody.vue'
import myfooter from './components/myfooter.vue'

export default {
  name: 'App',
  components: {
    myheader,
    compobody,
    myfooter,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
