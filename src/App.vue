<template>
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>|
    <router-link to="/contract">Contract</router-link>
    <Navbar></Navbar>
    <AllFriends :fri="friends"></AllFriends>
  </div>
  <router-view />
</template>

<style lang="stylus">
#app
  font-family Avenir, Helvetica, Arial, sans-serif
  -webkit-font-smoothing antialiased
  -moz-osx-font-smoothing grayscale
  text-align center
  color #2c3e50
  margin-top 60px
</style>
<script>
import Navbar from "@/views/Navbar";
import AllFriends from "@/views/AllFriends";
export default {
  data(){
    return {
      friends:[
        {name: 'A', online: true},
        {name: 'B', online: false},
        {name: 'C', online: true},
        {name: 'D', online: true},
        {name: 'E', online: false},
        {name: 'F', online: true},
        {name: 'G', online: true}
      ]
    }
  },
  components: {AllFriends, Navbar}
}
</script>