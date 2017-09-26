<template>
  <div class="chat" >
    <div class="chat-list">
      <userInfo></userInfo>
      <listBar></listBar>
      <list></list>
    </div>

    <div class="chat-window">
      <winHead></winHead>
      <winMain></winMain>
      <winFoot></winFoot>
    </div>
  </div>
</template>

<script>
import userInfo from './ChatWindow/ChatUserInfo'
import listBar from './ChatWindow/ChatListBar'
import list from './ChatWindow/ChatList'
import winHead from './ChatWindow/ChatWinHead'
import winMain from './ChatWindow/ChatWinMain'
import winFoot from './ChatWindow/ChatWinFoot'
export default {
  name: 'hello',
  data () {
    return {
      chat_infos: [
        {
          id: 0,
          img_src: require('../assets/test1.png'),
          chat_name: 'xxx',
          unread_num: 2,
          last_msg: '',
          is_notification: 0,
          time: '14:20'
        },
        {
          id: 1,
          img_src: require('../assets/test1.png'),
          chat_name: 'aaa',
          unread_num: 2,
          last_msg: '',
          is_notification: 0,
          time: '14:20'
        }
      ]
    }
  },
  components: {
    userInfo,
    listBar,
    list,
    winHead,
    winMain,
    winFoot
  }
}
</script>

<style scoped>
.chat{
  position: relative;
  width:900px;
  height:700px;
}
.chat-list{
  position: relative;
  width: 25%;
  height: 100%;
  float: left;
  background: #3a3a3a;
}
.chat-window{
  position: relative;
  width: 75%;
  height: 100%;
  float: left;
  background: #EEE;
}
</style>
