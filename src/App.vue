<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">首页</router-link>
      <router-link to="/about">about</router-link>
      <router-link to="/text">text</router-link>
    </div>
    <router-view/>
    <footes></footes>
  </div>
</template>

<script>
import footes from './components/footer'
export default {
  name: 'app',
  components: {
    footes: footes
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
  margin-top: 60px;
}

#nav{
  width: 100%;
  background: rgb(215, 230, 9);
  margin-top: -60px;
}
#nav a{
   display:inline-block;
   width: 30%;
   height: 50px;
   margin-top: 20px;
  }
</style>
