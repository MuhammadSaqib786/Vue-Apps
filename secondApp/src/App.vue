<template>
  <div id="app">
    <Header></Header>
    <router-view> </router-view>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import PostExample from './components/Posts.vue'
import Header from './components/Header'
import Contact from './components/Contact'

export default {
  name: 'App',
  components: {
    HelloWorld,
    PostExample,
    Header,
    Contact
  }
}
</script>

<style>

  @import "../node_modules/bootstrap/dist/css/bootstrap.min.css";

</style>
