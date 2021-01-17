<template>
  <el-container>
    <el-header>
      <Top />
    </el-header>
    <el-main>
      <Main/>
    </el-main>
    <el-footer>Footer</el-footer>
  </el-container>
</template>

<script>
import Top from "./components/Top.vue";
import Main from "./components/Main.vue";
export default {
  name: "App",
  components: {
    Top,
    Main
  },
};
</script>

<style>


.el-header,
.el-footer {
  /* background-color: #b3c0d1; */
  color: #333;
  text-align: center;
}
.el-header {
  line-height: 41px !important;;
  height: 41px !important;
}

.el-header>*{
  max-width: 990px;
  margin: 0 auto;
  padding-left: 20px;
}


.el-main {
  background-color: #e9eef3;
  color: #333;
  text-align: center;
  /* line-height: 160px; */
  padding: 0 !important;
}



body > .el-container {
  /* margin-bottom: 40px; */
}


</style>
