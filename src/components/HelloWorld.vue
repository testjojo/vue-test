<template>
  <div class="login">
    <div class="innerbox">
      <input class="account" placeholder="请输入账号"></input>
      <input class="password" placeholder="请输入密码"></input>
      <button @click="next">登录</button>
    </div>
    <div class="password"></div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  methods: {
    next() {

    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
  .login{
    width: 100%;
    height: 100%;
    background: url('../assets/back.jpg') no-repeat;
    position:absolute;
    .innerbox{
      width: 500px;
      height: 300px;
      background: #6778a9;
      text-align: center;
      position: fixed;
      right: 100px;
      top: 300px;
      .account, .password{
        display: block;
        margin: 0 auto;
        width: 280px;
        height: 40px;
        border-radius: 4px;
        margin-bottom: 5px;
        border: none;
        padding-left: 5px;
      }
      .account{
        margin-top: 50px;
      }
      button{
        width: 280px;
        margin-top: 50px;
        border-radius: 4px;
        height: 40px;
        outline: none;
        border:none;
        background: #00a0fe;
        color: #fff;
        cursor: pointer;
      }
    }
  }
</style>