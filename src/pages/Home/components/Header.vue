<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont back-icon">&#xe624;</div>
    </div>
    <div class="header-input">
      <span class="iconfont">&#xe632;</span>输入城市/景点/游玩/主题
    </div>
    <div class="header-right">
      城市
      <span class="iconfont">&#xe606;</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeHeader"
};
</script>

<style  scoped>
.header {
  display: flex;
  line-height: 2rem;
  background-color: #00bcd4;
  color: #fff;
  align-items: center;
}
.header-left {
  width: 10%;
  float: left;
}
.header-input {
  width: 70%;
  flex: 1;
  background-color: #fff;
  border-radius: 0.2rem;
  margin: 0.2rem;
  color: #ccc;
  padding: 0.2rem;
}
.header-right {
  width: 20%;
  text-align: center;
  display: flex;
  justify-content: center;
  align-items: center;
}
.back-icon {
  text-align: center;
}
</style>
