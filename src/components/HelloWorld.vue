<template>
  <el-container id="mainLayer">
    <el-header id="mainHeader">
      Header
    </el-header>
    <el-container>
      <el-aside id="mainAside" width="20%">Aside</el-aside>
      <el-container>
        <el-main id="mainMain">Main</el-main>
        <el-footer id="mainFooter">Footer</el-footer>
      </el-container>
    </el-container>
  </el-container>
</template>

<script>
export default {
  name: 'HelloWorld'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#mainLayer {
  height: 100%;
}
/*
#mainHeader,
#mainAside,
#mainMain,
#mainFooter {
  height: 10%;
  border: 1px solid #66b1ff;
  align-content: center;
} */
.el-header,
.el-footer {
  background-color: #b3c0d1;
  color: #333;
  text-align: center;
  line-height: 60px;
}
.el-aside {
  background-color: #d3dce6;
  color: #333;
  text-align: center;
  line-height: 200px;
}
.el-main {
  background-color: #e9eef3;
  color: #333;
  text-align: center;
  line-height: 160px;
}
body > .el-container {
  margin-bottom: 40px;
}
</style>
