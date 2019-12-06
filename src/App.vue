<template>
  <div id="app">
    <div class="header">
      <h1>多加网</h1>
    </div>
    <div class="ipt">
      <span class="iconfont icon-weibiaoti24"></span>
      <input type="text" placeholder="热门搜索" />
      <span>分类</span>
    </div>
    <div class="con">
      <router-view />
    </div>
    <div class="footer">
      <router-link to="/">
        <span class="iconfont icon-shoucang6"></span> 首页
      </router-link>
      <router-link to="/about">
        <span class="iconfont icon-wode1"></span> 我的
      </router-link>
    </div>
  </div>
</template>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  text-decoration: none;
  outline: none;
  border: none;
}
html,
body {
  width: 100%;
  height: 100%;
}
#app {
  width: 100%;
  height: 100%;
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  display: flex;
  flex-direction: column;
  .header {
    width: 100%;
    height: 40px;
    line-height: 40px;
    text-align: center;
    background: #000;
    color: #fff;
  }
  .ipt {
    width: 100%;
    height: 40px;
    line-height: 40px;
    display: flex;
    justify-content: space-around;
    background: green;
    span{
      flex: 2;
      text-align: center;
      color: #fff;
    }
    input{
      flex: 5;
      background: #fff;
      border-radius: 15px;
    }
  }
  .footer {
    width: 100%;
    height: 40px;
    line-height: 40px;
    display: flex;
    a {
      flex: 1;
      text-align: center;
      &.router-link-exact-active {
        color: #42b983;
      }
    }
  }
  .con {
    width: 100%;
    flex: 1;
    overflow: auto;
  }
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
