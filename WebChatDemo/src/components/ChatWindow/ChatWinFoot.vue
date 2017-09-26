<template>
  <div class="win-foot">
    <div class="msg-bar">
      <i class="el-icon-picture"></i>
      &nbsp;&nbsp;&nbsp;
      <i class="el-icon-document"></i>
    </div>
    <div class="msg-text">
      <textarea></textarea>
    </div>
    <div class="msg-foot">
      <span class="foot-text">Ctrl + Enter to Send </span>
      <el-button size="small">Send</el-button>
    </div>
  </div>
</template>
<script>
</script>
<style scope>
.win-foot{
  width: 100%;
  height: 35%;
}
.msg-bar{
  width:100%;
  height:10%;
  padding: 5px 17px;
}
.msg-text{
  width:100%;
  height:65%;
}
.msg-text textarea{
  padding: 10px;
  height: 100%;
  width: 100%;
  border: none;
  outline: none;
  font-family: "Micrsofot Yahei";
  resize: none;
}
.msg-foot{
  width:100%;
  height:30%;
  text-align: right;
  padding: 21px 0px;
}
.foot-text{
  display:inline;
  margin-left: 10px;
  margin-right: 7px;
  color: #888;
  font-size: 12px;
}
</style>