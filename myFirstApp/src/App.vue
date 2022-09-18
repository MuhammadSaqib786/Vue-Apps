<template>
  <div id="app">
    <Header></Header>
    <PostExample/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import PostExample from './components/Posts'
import Header from './components/Header'

export default {
  name: 'App',
  components: {
    HelloWorld,
    PostExample,
    Header
  }
}
</script>

<style>

  @import "../node_modules/bootstrap/dist/css/bootstrap.min.css";

</style>
