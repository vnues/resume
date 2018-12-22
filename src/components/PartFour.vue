<template>
  <div :class="partFive">
    <h3 class="text-center text-top">在校经历</h3>
    <p>
      <a href="javascript:void(0)">负责陶瓷学院网站的开发</a>
      <span class="text-small">| 2016/04 - 2016/6</span>
    </p>
    <p class="text-small">工作职责：负责编写前端页面以及交互</p>
    <p class="text-small">项目技术：</p>
    <p class="text-small">&emsp;1.使用html+css对UI图进行页面布局</p>
    <p class="text-small">&emsp;2. 与UI配合并对网站进行完善</p>
     <a  href="http://tcxy.hstc.edu.cn" target="_blank">项目地址：http://tcxy.hstc.edu.cn</a>
  </div>

</template>

<script>
export default {
  name: "partFive",
  data() {
    return {
      partFive: "part-five",
      curWidth: 0
    };
  },
  beforeMount() {
    this.curWidth = document.documentElement.clientWidth || document.body.clientWidth;
    if(this.curWidth < 1600) {
      this.partFive = "part-five-responsive"
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
.part-five {
  width: 100%;
  height: 310px;
  border: 40px solid transparent;
  border-image: url("~@/./assets/img/border_image.png") 30 30 stretch;
  background: #18202d;
}
.part-five-responsive {
  width: 100%;
  border: 40px solid transparent;
  border-image: url("~@/./assets/img/border_image.png") 30 30 stretch;
  background: #18202d;
}
.text-center {
  text-align: center;
}
.text-small {
  font-size: 0.9em;
  color: rgb(253, 239, 239);
}
</style>