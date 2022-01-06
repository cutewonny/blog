<template>
  <div>
      <h5>{{블로그글[0].title}}</h5>
      <p>{{블로그글[0].content}}</p>
  </div>
  <div>
      <h5>{{블로그글[1].title}}</h5>
      <p>{{블로그글[1].content}}</p>
  </div>
  <div>
      <h5>{{블로그글[2].title}}</h5>
      <p>{{블로그글[2].content}}</p>
  </div>
  
</template>

<script>
export default {
    name: 'List',
    props:{
        블로그글 : Array,
    },
    data(){
        return{
           
        };
    }
}
</script>

<style>

</style>