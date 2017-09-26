<template>
  <div class="win-main">
    <div>
        <ul>
          <li v-for="chatMsg in chatMsgs"  :key="chatMsg.id">
            <p class="msg-time"><span>{{chatMsg.time}}</span></p>
            <div :class="{'chat-msg-other': !chatMsg.isUser, 'chat-msg-self': chatMsg.isUser}">
              <img class="chat-avatar" :src="chatMsg.user_avatar">
              <div class="msg">
                <h4>{{chatMsg.user}}</h4>
                <div class="msg-text">{{chatMsg.msg}}</div>
              </div>
            </div>
          </li>
        </ul>
    </div>
  </div>
</template>
<script>
export default{
  data () {
    return {
      chatMsgs: [{
        id: 0,
        msg: '测试信息，啦啦啦啦啊啊啊啊哈哈哈哈嘿嘿和',
        user: '222',
        user_avatar: require('../../assets/test1.png'),
        time: '12:20',
        isUser: true,
        success: 1
      }, {
        id: 1,
        msg: '测试信息，啦啦啦啦啊啊啊啊哈哈哈哈嘿嘿和',
        user: '222',
        user_avatar: require('../../assets/test1.png'),
        time: '',
        isUser: false,
        success: 1
      }, {
        id: 2,
        msg: '111',
        user: '222',
        user_avatar: require('../../assets/test1.png'),
        time: '',
        isUser: false,
        success: 1
      }]
    }
  }
}
</script>
<style scope>
.win-main{
  width: 95%;
  height: 60%;
  background-color:#DDD;
  padding: 15px 15px;
  overflow-y: scroll;
}
.msg-time{
  margin: 7px 0;
  text-align: center;
}
.msg-time span{
  display: inline-block;
  padding: 0 18px;
  font-size: 12px;
  color: #fff;
  border-radius: 2px;
  background-color: #dcdcdc;
}
.chat-msg-other{
  
}
.chat-msg-other .text{
  display: inline-block;
  position: relative;
  padding: 0 10px;
  max-width:100%;
  min-width:40px;
  min-height: 30px;
  line-height: 2.5;
  font-size: 12px;
  text-align: left;
  word-break: break-all;
  background-color: #fafafa;
  border-radius: 4px;
}
.chat-msg-self{
  width: 100%;
}
.chat-avatar{
  width:50px;
  height:50px;
  float: left;
  margin: 0 10px 0 0;
  border-radius: 3px;
}
li {
  list-style: none;
}
</style>