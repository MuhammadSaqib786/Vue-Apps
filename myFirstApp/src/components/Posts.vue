<template>
<div  class="container">
    <h3>
        Hi.. Welcome Saqib to your first component
    </h3>
    Below data from jsonplaceholder API:
    <table class="table table-success mt-4">
  <thead>
    <tr>
      <th scope="col">UserId</th>
      <th scope="col">Id</th>
      <th scope="col">Title</th>
      <th scope="col">Body</th>
    </tr>
  </thead>
  <tbody>
    <tr v-for='post in posts' @key="post.id">
      <th scope="row">{{post.id}}</th>
      <td>{{post.title}}</td>
      <td>{{post.body}}</td>
    </tr>
    
  </tbody>
</table>
    
    <button class="btn btn-primary">Let's Get Started</button>
</div>
</template>

<script>
export default{

    name: 'PostExample',
    data(){
        return{
            posts:[
                
            ]
        }
    }
}

</script>

<style>

</style>