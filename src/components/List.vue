<template>
  <div>
      <h5>{{blogTitle}}</h5>
      <p>{{blogContent}}</p>
      <h5>{{블로그글.title}}</h5>
      <p>{{블로그글.content}}</p>
  </div>
  
</template>

<script>
export default {
    name: 'List',
    props:{
        블로그글:Array,
    },
    data(){
        return{
            blogTitle : '블로그 글 제목',
            blogContent: '블로그 글 내용',
        };
    }
}
</script>

<style>

</style>