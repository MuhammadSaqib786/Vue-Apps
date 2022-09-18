<template>
<div>
    <h3>
        Hi.. Welcome Saqib to your first component
    </h3>
    Below are some langauges you should learn:
    <ul>
        <li v-for='post in posts' @key="id">{{post.title}}</li>
    </ul>
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