<template>
  <div class="list-bar">
    <div class="search-bar">
      <input class="search" type="text" placeholder="search user..." >
    </div>
    <!--<div class="tab-bar">
      <div class="tab-bar-item">
        <a>
          <i class="el-icon-message" ></i>
        </a>
      </div>
      <div class="tab-bar-item">
        <a>
          <i class="el-icon-message"></i>
        </a>
      </div>
      <div class="tab-bar-item">
        <a>
          <i class="el-icon-message"></i>
        </a>
      </div>
    </div>-->
  </div>
</template>
<script>
</script>
<style scope>
.list-bar{
  width: 100%;
  height: 5%;
}
.search-bar{
  height:100%;
}
.search{
  padding: 0 10px;
  width: 100%;
  font-size: 12px;
  color: #fff;
  height: 30px;
  line-height: 30px;
  border: solid 1px #3a3a3a;
  border-radius: 4px;
  outline: none;
  background-color: #26292E;
}
.tab-bar{
  height:50%;
  overflow: hidden;
  position: relative;
  padding-bottom: 4px;
}
.tab-bar-item{
  float: left;
  width: 33.33333333%;
  position: relative;
  display: block;
  text-align: center;
}
.tab-bar-item :after{
  content: '';
  position: absolute;
  top: 7px;
  right: 0;
  width: 0;
  height: 20px;
  border-right: 1px solid #000;
}
</style>