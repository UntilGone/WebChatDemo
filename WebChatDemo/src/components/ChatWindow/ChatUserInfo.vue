<template>
  <div class="user-info">
    <img class="avatar" :alt="user.name" :src="user.img">
    <p class="name">{{user.name}}</p>
  </div>
</template>
<script>
export default{
  data () {
    return {
      user: {
        name: 'NULL',
        img: require('../../assets/test1.png')
      }
    }
  }
}
</script>
<style scope>
.user-info{
  width: 100%;
  height: 8%;
  background-color:#333;
  padding: 6%;
  border-bottom: solid 1px #24272C;
}
.avatar{
  vertical-align: middle;
  border-radius: 2px;
  width:50px;
  height:50px;
}
.name{
  vertical-align: middle;
  display: inline-block;
  margin: 0 0 0 15px;
  font-size: 16px;
  color: #fff;
}
</style>