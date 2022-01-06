<template>
<button type="button" class="btn btn-primary">Primary</button>
<button type="button" class="btn btn-secondary">Secondary</button>
<button type="button" class="btn btn-success">Success</button>
<button type="button" class="btn btn-danger">Danger</button>
<button type="button" class="btn btn-warning">Warning</button>
<button type="button" class="btn btn-info">Info</button>
<button type="button" class="btn btn-light">Light</button>
<button type="button" class="btn btn-dark">Dark</button>

<button type="button" class="btn btn-link">Link</button>
<!-- <List :blogData="blogData" v-for="i in 3"  :key="i"/> -->
<List :블로그글="blogData[i]" v-for="(bd,i) in blogData"  :key="bd"/>
{{data}}
</template>

<script>
import List from './components/List.vue'
import {data} from './assets/data.js'
console.log(data)
export default {
  name: 'App',
  data(){
    return{
      blogData : data,
    }

  },
  components: {
    List:List,
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
