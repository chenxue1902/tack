<!--  -->
<template>
<div class='Login'>
    <!-- 登录广告图片 -->
    <img class="login-Img" src="../assets/login-img.ca4e6fe.png" /> 
    <!-- 登录框 -->
    <div class="loginFrame">
        <h1>领课教育系统-开源版</h1>
        <div class="loginSystem">
            <i class="el-icon-user-solid" ></i>
            <el-input v-model="input" placeholder="请输入内容"></el-input>
        </div>
        <div class="loginSystem">
            <i class="el-icon-s-goods" ></i>
             <el-input placeholder="请输入密码" v-model="pass" show-password></el-input>
        </div>
        <el-button type="primary">登录</el-button>
    </div>
    <!-- 个人用户头像 -->
    <div class="loginUser">
        <i class="el-icon-user"></i>
    </div>
    <!-- 企业商标 -->
    <ul class="loginDescribe">
        <li>广州市领课网络科技有限公司</li>
        <li>版权所有2015-2019</li>
        <li>|粤ICP备16009964号</li>
    </ul>
</div>
</template>

<script>
//这里可以导入其他文件（比如：组件，工具js，第三方插件js，json文件，图片文件等等）
//例如：import 《组件名称》 from '《组件路径》';

export default {
//import引入的组件需要注入到对象中才能使用
components: {},
data() {
//这里存放数据
return {
  input:'',
  pass: ''
};
},
//监听属性 类似于data概念
computed: {},
//监控data中的数据变化
watch: {},
//方法集合
methods: {

},
//生命周期 - 创建完成（可以访问当前this实例）
created() {

},
//生命周期 - 挂载完成（可以访问DOM元素）
mounted() {

},
beforeCreate() {}, //生命周期 - 创建之前
beforeMount() {}, //生命周期 - 挂载之前
beforeUpdate() {}, //生命周期 - 更新之前
updated() {}, //生命周期 - 更新之后
beforeDestroy() {}, //生命周期 - 销毁之前
destroyed() {}, //生命周期 - 销毁完成
activated() {}, //如果页面有keep-alive缓存功能，这个函数会触发
}
</script>
<style lang='scss' scoped>
//@import url(); 引入公共css类
.Login{
    width: 100%;
    height: 100%;
    position: absolute;
    background: #93defe;
}
.login-Img{
    width: 300px;
    height: 280px;
    margin-left: 160px;
    margin-top: 120px;
}
.loginFrame{
    width: 280px;
    height: 260px;
    display: flex;
    justify-content: space-around;
    flex-direction: column;
    align-items: center;
    background: white;
    position: absolute;
    top: 120px;
    right: 160px;
    border-radius:5px;
    h1{
        font-size: 20px;
        margin-top: 40px;
    }
}
.loginUser{
    width: 80px;
    height: 80px;
    border: 3px solid #93defe;
    background: white;
    border-radius: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    position: absolute;
    right: 258px;
    top: 80px;
    i{
        font-size: 50px;
        color: #93defe;
    }
}
.loginSystem{
    display: flex;
    width: 80%;
    height: 40px;
    background: #E5E5E5;
    justify-content: space-around;
    align-items: center;
    border-radius: 5px;
    i{
        margin-right: 10px;
        margin-left: 10px;
        color: #889AA4;
    }
    .el-input{
        background-color: #E5E5E5;
    }
}
.loginDescribe{
    list-style: none;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 13px;
    color: white;
    position: absolute;
    top: 430px;
    width: 100%;
    height: 20px;
    li{
        margin-left:10px;
    }
}
</style>