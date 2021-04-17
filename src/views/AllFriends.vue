<template>
  <div id="allfriends">
    <h2>All Friends</h2>
    <div v-for="(friend,index) in fri" :key="index">
      <h6 v-if="friend.online">{{ index+1 }}.{{ friend.name}}</h6>
    </div>
  </div>
</template>

<script>export default {
  name:"AllFriends",props:["fri"],
};
</script>
<style scoped>
</style>