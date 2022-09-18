<template>
  <div id="app">
    
    <PostExample/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import PostExample from './components/Posts'

export default {
  name: 'App',
  components: {
    HelloWorld,
    PostExample
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
</style>
