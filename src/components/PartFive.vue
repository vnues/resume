<template>
  <div :class="partFive">
    <h3 class="text-center text-top">实习经验</h3>
    <p>
      <a href="javascript:void(0)">潮州蓝梦科技有限公司</a>
      <span class="text-small">| 2017/02 - 2018/11</span>
    </p>
    <p class="text-small">工作内容：日常操作 jQuery 编写活动页、微信商城</p>
    <p class="text-small">项目成就：</p>
    <p class="text-small">&emsp;1. 微信商城。使用jquery进行微信商城的开发，项目已完成，商城已下架</p>
    <p class="text-small">&emsp;2. 微信一元云购，使用vue开发一元云购，项目已完成，已下架</p>
    <p class="text-small">&emsp;3. jQuery 活动页及 H5 活动页。</p>
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