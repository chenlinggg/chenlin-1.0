<template>
  <div id="app">
    <!-- 顶部导航栏 -->
   <nav class="topbar">
   <div class="topbar-left">
      <img src="./image/龙.png">
      <p>陈林</p>
   </div>
   
  <div class="topbar-right">
     <ul>
     <li><a href="#">主页</a></li>
     <li><a href="#">技能</a></li>
     <li><a href="#">作品</a></li>
     <li><a href="#">教育</a></li>
     <li><a href="#">关于</a></li>
     </ul>
</div>

   </nav>


   <!--中间的部分-->
   <div class="content">
    <!--中间的左边的部分-->
   <div class="conten-left">
    <p>欢迎来到我的博客</p>
    <p>下面是本人的联系方式</p>
    <p>联系电话：17385403147，邮箱：1489789468@qq.com</p>
    <button>继续浏览</button>
   </div>
   <div class="conten-left">
    <img src="./image/content-image.png">
     
   </div>
         

   </div>
   <!--中间的部分结束-->



   <!-- 技能的首页 -->
  <div class="center-banxin skill-page-box height-780px">
    <div class="skill-page"  v-for="item in 9" :key="item">
     <div class="skill-page-left">
      <i class="iconfont icon-Vue"></i>
      <p class="font-YuanFeng-22">vue</p>
    
     </div>
     <div class="skill-page-left">
      <p class="font-YuanFeng-22">技能一：</p>
      <p class="font-YuanFeng-22">熟悉vue2全家桶：vueRouter，vuex，Axios等</p>
     </div>
  </div>
  </div>





  </div>
</template>

<script>


export default {
  name: 'App',
  components: {
 
  }
}
</script>

<style>
#app{
  background-image: linear-gradient(to right, #a8edea 0%, #fed6e3 100%);
   height: auto;
}
.height-780px{
  height: 780px;
}
.skill-page-box{
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  align-content: space-between;
  
}
.icon-Vue{
     
      width: 100px;
      height: 40px;

}
.skill-page{
  border: 1px solid red;
  background-color:rgba(103, 70, 223, 0.875);
  border-radius: 9px;
  width: 450px;
  height: 100px;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  align-content: center;
}
/* 这个是中间的样式 */
.conten-left p{
  font-family: YuanFeng;
  font-size: 27px;
}
.conten-left button{
            border-radius: 2rem;
           width:120px;
          height: 32px;
          font-family: YuanFeng;
          font-size: 21px;
}
.conten-left button:hover{
  background-color: #a8edea;
  color: rgba(255, 255, 255, 0.875);
}

.content{
  width: 1000px;
  border: 1px solid red;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  margin-top: 20px;
}
.conten-left img{
  width: 400px;
  height: 400px;
  animation-name:changAppea;
  animation-duration: 2s;
  animation-timing-function: ease;
}
.conten-left img:hover{
  transform: scale(1.01);
}
@keyframes changAppear{
   0%{
   opacity: 0;
   }
   100%{
    opacity: 1;
   }
 }
.conten-left{
  display: flex;
  flex-direction: column;
  justify-content: center;

}
/* 顶部的导航栏的样式 */
.topbar{
  width: 1000px;
  border: 1px solid red;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
}
.topbar-left{
  width: 90px;
  display: flex;
  justify-content: space-between;
}

.topbar-left img{
 width: 28px;
 height: 28px;
}
.topbar-left p{
 
  font-family: YuanFeng;
  font-size: 21px;

}
 
.topbar-right ul{
  list-style: none;
  display: flex;
}
.topbar-right ul li{
  margin-right: 20px;
}
.topbar-right ul li>a{
  text-decoration: none;
  font-family: YuanFeng;
  font-size: 22px;
  color:black;
  
}
.topbar-right ul li>a:hover{
  background-color:#f38181;
  border-radius: 1rem;
  color: #eaffd0;

}


</style>
