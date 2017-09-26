<template>
  <div class="list">
    <ul>
      <li v-for="msg_info in msg_infos" :key="msg_info.id">
        <img class="avatar" :alt="msg_info.chat_name" :src="msg_info.img_src">
        <p class="name">{{msg_info.chat_name}}</p>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  data () {
    return {
      msg_infos: [
        {
          id: 0,
          img_src: require('../../assets/test1.png'),
          chat_name: 'xxx',
          unread_num: 2,
          last_msg: '',
          is_notification: 0,
          time: '14:20'
        },
        {
          id: 1,
          img_src: require('../../assets/test1.png'),
          chat_name: 'aaa',
          unread_num: 2,
          last_msg: '',
          is_notification: 0,
          time: '14:20'
        }
      ]
    }
  }
}
</script>
<style scope>
.list {
  width: 100%;
  height: 83%;
  background-color: #444;
}

.list li {
  list-style: none;
  padding: 12px 15px;
  border-bottom: 1px solid #292C33;
  cursor: pointer;
  transition: background-color .1s;
}

.list li:hover {
  background-color: rgba(255, 255, 255, 0.03);
}

.avatar,
.name {
  vertical-align: middle;
}

.name {
  display: inline-block;
  margin: 0 0 0 15px;
}

ul {
  margin: 0;
  padding: 0;
}
</style>