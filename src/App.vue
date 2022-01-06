<template>

<!-- <List :blogData="blogData" v-for="i in 3"  :key="i"/> -->
<!-- <List :블로그글="blogData[i]" v-for="(bd,i) in blogData"  :key="bd"/> -->

<router-link to="/">Home</router-link>
<router-link to="/list"> 리스트 페이지</router-link>
<!-- <router-view :블로그글="blogData[i]" v-for="(bd,i) in blogData" :key="bd"></router-view> -->
<router-view :블로그글="blogData"></router-view>

<p>{{blogData}}</p>
</template>

<script>
// import List from './components/List.vue'
import data from './assets/data.js'

export default {
  name: 'App',
  data(){
    return{
      blogData : data,
    }

  },
  components: {
    // List:List,
  },
  
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
