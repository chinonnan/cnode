<template>
  <div id="app">
    <Header></Header>
    <div class="main">
      <router-view name="slidebar"></router-view>
      <router-view name='main'></router-view>
      <!-- <PostList></PostList> -->
    </div>

  </div>
</template>

<script>
import Header from './components/Header'
import PostList from './components/PostList'
export default {
  name: 'App',
  components:{
    Header,
    PostList
  }
}
</script>

<style>
.main{
  width: 80%;
  margin: 0 auto;
}
  #app{
    background-color: #e1e1e1;
  }
</style>
