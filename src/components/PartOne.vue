<template>
  <div class="part-one">
    <img class="part-one-image" :src="headImage" alt="头像">
    <p>姓&emsp;&emsp;名：Vnues</p>
    <p>学&emsp;&emsp;历：本科</p>
    <p>期待职位：Web前端</p>
    <p>年&emsp;&emsp;龄：22</p>
    <p>联系电话：15363393850</p>
    <p>电子邮箱：1518190293@qq.com</p>
    <p>博&emsp;&emsp;客：<a href="www.wgfvnues.mobi:3000" target="_blank">我的个人博客</a></p>
    <p>GitHub：<a href="https://github.com/vnues" target="_blank">vnues</a></p>
  </div>
</template>

<script>
export default {
  name: "partOne",
  data() {
    return {
      headImage: require('../assets/img/head_image.png')
    }
  }
};
</script>

<style scoped>
a {
  color: deepskyblue;
}
a:hover {
  color: rgb(118, 190, 248);
}
p {
  line-height: 30px;
}
.part-one {
  width: 100%;
  height: 500px;
  border: 40px solid transparent;
  border-image: url("~@/./assets/img/border_image.png") 30 30 stretch;
  background: #18202d;
  padding-left: 10px;
}
.part-one-image {
  width: 150px;
  height: 150px;
}
</style>