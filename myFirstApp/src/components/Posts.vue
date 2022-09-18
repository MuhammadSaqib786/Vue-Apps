<template>
<div  class="container">
    <h3>
        Hi.. Welcome Saqib to your first component
    </h3>
    Below are some langauges you should learn:
    <table class="table table-success mt-4">
  <thead>
    <tr>
      <th scope="col">Id</th>
      <th scope="col">Language</th>
    </tr>
  </thead>
  <tbody>
    <tr v-for='post in posts' @key="id">
      <th scope="row">{{post.id}}</th>
      <td>{{post.title}}</td>
      
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
                {id:1,title:'C++'},
                {id:2,title: 'Java'},
                {id:3,title:'Python'},
                {id:4,title: 'C#'},
                {id:5,title:'VB'},
                {id:6,title: 'Kotlin'},
            ]
        }
    }
}

</script>

<style>

</style>