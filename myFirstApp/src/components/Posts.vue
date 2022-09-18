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
      <th scope="col">Usage</th>
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
                {id:1,title:'C++',body:'This is simple langauge to start learn programming.'},
                {id:2,title: 'Java',body:'This is more advanced langauge.'},
                {id:3,title:'Python',body:'Best langauge used for machine learning and AI.'},
                {id:4,title: 'C#',body:'Best for web app development purposes'},
                {id:5,title:'VB',body:'Thats also alternate to C# langauge.'},
                {id:6,title: 'Kotlin',body:'Best langauge used now a days for android application development.'},
            ]
        }
    }
}

</script>

<style>

</style>