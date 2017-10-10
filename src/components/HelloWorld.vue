<template>
  <div>

  <div class="top">

    <div class="img">
      <img src="../assets/1.jpg" width="160">
    </div>

   <div class="menu">
     <ul>
       <li><a href="#">课程 </a></li>
       <li><a href="#">职业路径</a></li>
       <li><a href="#">实战</a></li>
       <li><a href="#">猿问</a></li>
       <li><a href="#">手记</a></li>
     </ul>
   </div>

    <div class="serach">
      <a>前端入门</a>
      <a>Java入门</a>
    </div>

    <div><a>下载APP</a></div>

    <div><button>购物车</button></div>

    <div><img src="../assets/2.png" width="35px"></div>
  </div>



  </div>
</template>

<script>


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style >
  *{
    padding:0;
    margin:0;;
  }
  .top{
    width:100%;
    height:72px;
    background-color: #fff; 
  }
  .img{
    margin:10px 30px;
    float: left;
    display: block;
  }
  .menu li{
    float: left;
    list-style-type: none;
    padding-left: 20px;
    padding-right: 10px;
    text-align: center;
    line-height: 72px;
    display: block;
  }
  .menu a:link,.menu a:visited{
    text-decoration: none;
    color: #333;
    font-size: large;
  }
  .menu a:hover,.menu a:active{
    color: #000;
  }
  .serach a{
    border: 1px solid;
    border-radius: 25px;
    width: 100px;
    height:25px;
    float: left;

  }
</style>
