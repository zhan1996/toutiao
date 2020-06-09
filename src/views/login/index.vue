<template>
    <div class="container-login">
      <el-card>
          <img class="logo" src="../../assets/logo_index.png" alt="">
          <el-form>
              <el-form-item>
                  <el-input v-model="loginForm.mobile" placeholder="请输入手机号"></el-input>
              </el-form-item>
              <el-form-item>
                  <el-input style="width:240px; margin-right:8px" palceholder=""></el-input>
                <el-button>发送验证码</el-button>
              </el-form-item>
              <el-form-item>
                  <el-checkbox :value="true">我已阅读并同意用户协议和隐私条款</el-checkbox>
              </el-form-item>
              <el-form-item>
                  <el-button type="primary" style="width:100%">登 录</el-button>
              </el-form-item>
          </el-form>
      </el-card>
    </div>
</template>
           
<script>
export default{
      name:'login-page',
      data(){
          return {
              loginForm:{
                  mobile:'',
                  code:''
              }
          }
      }       
}
</script>
<style scoped lang="less">
   .container-login {
       width: 100%;
       height: 100%;
       background: url(./../../assets/bg3.jpg) no-repeat center / cover;
       position: absolute;
       left: 0;
       top: 0;
       .el-card {
           width: 400px;
           height: 350px;
           position: absolute;
           left: 50%;
           top: 50%;
           transform: translate(-50%,-50%);
           .logo {
               width: 200px;
               display: block;
               margin: 0 auto 20px;
           }
       }
   }         
</style>