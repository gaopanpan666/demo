
<template>

  <div class="hello">
    <div class="home_tit"></div>
    <div class="left-hand"></div> 
    <div class="person">
      <router-link :to="{name:'q1' , query:{type:1},params:{step:1}}"><div class="f-like"></div></router-link>
      <router-link :to="{name:'q1' , query:{type:0},params:{step:1}}"><div class="f-wenke"></div></router-link>
    </div>
    <div class="right-hand"></div>
  </div>
</template>
<script>
export default {
  

}
</script>

<style>
.hello{
    width:100%;
    height:100%;
    display:flex;
  }
  .home_tit{
    position: absolute;
    height:60px;
    width: 50%;
    left:26%;
    background: url('../../static/imgs/home-title.png') no-repeat;
    background-size: 100% 100%;
    top: 50px;
  }
  .person{
    width:80%;
    height:11rem;
    margin:0 auto;
    background:pink;
    background: url(../../static/imgs/home-pepole.png) no-repeat;
    background-size: 100%;
    display: flex;
  }
  .person a{
    display: block;
    width:100%;
    height:40%;
    margin-top:60%;
    position: relative;
  }
  .person .f-like{
    width:100%;
    height:40%;
    background:pink;
    background:url(../../static/imgs/f-like.png) no-repeat;
    background-size:90%;
    position:absolute;
    top:30%;
    left:10%;
  }
  .person .f-wenke{
    width:100%;
    height:40%;
    background:blue;
    background:url(../../static/imgs/f-wenke.png) no-repeat;
    background-size:80%;
    position:absolute;
    top:30%;
    left:10%;
  }
  .left-hand{
    width:10%;
    height:70%;
    background: url(../../static/imgs/home-left-hand.png) no-repeat;
    background-position: 0 80%;
    background-size:100%;
    
  }
  .right-hand{
    width:10%;
    height:70%;
    background: url(../../static/imgs/home-right-hand.png) no-repeat;
    background-position: 0 80%;
    background-size:100%;
    
  }
</style>
