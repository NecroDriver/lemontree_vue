<template>
  <el-container>
    <el-header class="header">
      <h1>have a try</h1>
    </el-header>
    <el-main class="main">
      <div class="login">
        <h2>登 陆</h2>
        <input name="account" type="text" placeholder="账户" required/>
        <input name="password" type="password" placeholder="密码" required/>
        <div class="tick">
          <input type="checkbox" id="brand" style="display: none"/>
          <label for="brand" id="remember">
            <span></span>记住我
          </label>
        </div>
        <div class="button">
          <input type="button" value="登 陆" @onclick="login"/>
        </div>
        <a href="#">记住密码？</a>
        <div class="social-login">
          <p>- 其他登陆方式 -</p>
          <ul>
            <li class="qq">
              <a href="#">
                <span class="icons"></span>
                <span class="text">QQ</span>
              </a>
            </li>
            <li class="weixin w3ls">
              <a href="#">
                <span class="icons w3layouts"></span>
                <span class="text">微信</span>
              </a>
            </li>
            <li class="weibo aits">
              <a href="#">
                <span class="icons agileits"></span>
                <span class="text">微博</span>
              </a>
            </li>
          </ul>
        </div>
        <div class="clear"></div>
      </div>
      <div class="line"></div>
      <div class="register"></div>
      <div class="clear"></div>
    </el-main>
    <el-footer>foot</el-footer>
  </el-container>
</template>

<script>
export default {
  name: 'Login'
}
</script>

<style scoped lang="less">
@import "../common/less/variable";
.header {
  font-size: 45px;
  font-weight: 500;
  letter-spacing: 4px;
  margin: 60px 0;
}
.main {
  width: 50%;
  margin: 0 auto;
  padding: 40px;
  background-color: #222222;
  border: 2px ridge rgba(238, 238, 238, 0.13);
  border-radius: 5px;
  -moz-box-shadow: 0 -5px 10px 1px rgba(16, 16, 16, 0.57);
  -webkit-box-shadow: 0 -5px 10px 1px rgba(16, 16, 16, 0.57);
  box-shadow: 0 -5px 10px 1px rgba(16, 16, 16, 0.57);
  border-bottom: none;
  border-bottom-left-radius: initial;
  border-bottom-right-radius: initial;
}
.login {
  width: 45%;
  float: left;
  text-align: left;
  padding-right: 40px;
  h2 {
    font-size: 35px;
    text-align: left;
    color: #FFF;
    font-weight: 100;
    margin-bottom: 20px;
  }
  input[type="text"],input[type="password"] {
    width: 93.4%;
    margin-bottom: 20px;
    padding: 10px;
    float: left;
    background-color: transparent;
    border: none;
    font-size: @font-size-medium;
    border-bottom: 1px solid rgba(238, 238, 238, 0.41);
    outline: none;
    color: #FFF;
  }
  .tick {
    float: left;
    display: inline-block;
    width: 100%;
    margin-bottom: 20px;
    input[type="checkbox"] + label {
      position: relative;
      padding-left: 30px;
      border: #F0F8FF;
      display: inline-block;
      font-size: @font-size-small;
      color: #EEE;
      span:first-child {
        width: 17px;
        height: 17px;
        display: inline-block;
        border: 1px solid #EEE;
        position: absolute;
        top: -3px;
        left: 0;
        bottom: 4px;
      }
    }
  }
  .button {
    margin-bottom: 20px;
    input[type="button"] {
      width: 60%;
      padding: 10px 0;
      font-size: @font-size-medium-x;
      font-weight: 100;
      background-color: transparent;
      color: #CCC;
      border: 1px solid rgba(238, 238, 238, 0.41);
      border-width: thin;
      cursor: pointer;
      outline: none;
      -webkit-transition: 0.5s all;
      -moz-transition: 0.5s all;
      -ms-transition: 0.5s all;
      -o-transition: 0.5s all;
      transition: 0.5s all;
      text-decoration: none;
    }
  }
  a {
    color: #CCC;
  }
  .social-login {
    margin-top: 20px;
    text-align: center;
    p {
      color: #CCC;
      margin-bottom: 15px;
    }
  }
}

</style>
