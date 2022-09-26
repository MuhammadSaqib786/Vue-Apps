<template>
<div  class="container">
    <h3>
        Hi.. Welcome Saqib to your first component
    </h3>
    Below data from jsonplaceholder API:
    <table class="table table-success table-responsive mt-4">
  <thead>
    <tr>
      <th scope="col">albumId</th>
      <th scope="col">Id</th>
      <th scope="col">Title</th>
      <th scope="col">Image</th>
    </tr>
  </thead>
  <tbody>
    <tr v-for='post in posts' @key="post.id">
      <th scope="row">{{post.albumId}}</th>
      <td>{{post.id}}</td>
      <td>{{post.title}}</td>
      <td><img :src="post.url" alt="img" class="img" height="200px"></td>
    </tr>
    
  </tbody>
</table>
    
    <button class="btn btn-primary">Let's Get Started</button>
</div>
</template>

<script>
    import axios from 'axios';
export default{

    name: 'PostExample',
    data(){
        return{
            posts:[
                
            ]
        }
    },
    created()
    {
        axios.get('https://jsonplaceholder.typicode.com/photos').then(posts=>{
            this.posts=posts.data
        });
    }
}

</script>

<style>

</style>