<template>
  <el-row type="flex" class="row-bg" justify="space-between">
    <el-col :span="9">
      <div class="grid-content bg-purple">
        <a href="#" class="logo"
          ><img src="../assets/images/logo.png" alt=""
        /></a>
        <span>
          <img src="../assets/images/img_01.jpg" alt="" />
          <a href="#"><img src="../assets/images/img_02.jpg" alt="" /></a>
        </span>
      </div>
    </el-col>
    <el-col :span="7">
      <div class="grid-content bg-purple-light right">        
          <h3 class="text1"><a href="#">成长守护平台</a></h3>
          <h3 class="text2">
            <span>腾讯游戏排行榜</span>
            <iframe
              src="https://game.gtimg.cn/images/js/title/title_game_rank.html?rd=0.76427870921507"
              frameborder="0"
            ></iframe>
          </h3>        
      </div>
    </el-col>
  </el-row>
</template>

<script>
export default {
  name: "Top",
};
</script>

<style>
.el-row {
  width: 1200px !important;
  &:last-child {
    margin-bottom: 0;
  }
}
.grid-content {
  height: 41px;
}
.logo {
  margin-right: 20px;
  position: relative;
  z-index: 11;
}
span a {
  position: absolute;
  left: 0;
  top: 0;
  z-index: 10;
  display: none;
}

span:hover a {
  display: block;
}

.right{
    align-items: center;
    position: relative;
    display: flex;
}

.right h3{
    color: #464646;
    font-size: 14px;
    line-height: 40px;
    font-weight: normal;

    position: relative; /* 为了放小图标 */
}
.right h3 a{
    color: #464646;
}
.right h3 a:hover{
    color: #ff4e00;
}
.right h3.text1{
    margin-right: 20px;
    padding-left: 30px;
}
.right h3.text1::before{
    content: '';    /* 内容 */
    width: 30px;
    height: 30px;
    background: url(/src/assets/images/ico_01.png) -30px 0;
    /* background: chartreuse; */
    position: absolute;
    left: 0;
    top: 5px;
}
.right h3.text2{
    padding-right: 30px;
    cursor: pointer;
}
.right h3.text2::after{
    content: '';    /* 内容 */
    width: 30px;
    height: 30px;
    background: url(/src/assets/images/ico_01.png);
    /* background: red; */
    position: absolute;
    right: 5px;
    top: 5px;

    transform: rotate(90deg);
    opacity: .1;    /* 透明度 */
}
.right iframe{
    width: 708px;
    height: 582px;
    position: absolute;
    top: 40px;
    right: 20px;
    z-index: 11;
    display: none;
}
.right h3.text2:hover iframe{
    display: block;
}
</style>



