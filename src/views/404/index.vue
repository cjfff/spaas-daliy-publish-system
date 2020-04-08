<template>
  <div class="error-wrapper">
    <div>
      <img
        src="//deepexi.oss-cn-shenzhen.aliyuncs.com/deepexi-services/%E5%85%AC%E5%85%B1/404.png"
        width="440px"
      />
      <br />
      <div class="text">抱歉，你访问的页面不存在。</div>
    </div>
    <el-button @click="goHome" type="primary" round>返回首页</el-button>
  </div>
</template>

<script>
export default {
  methods: {
    goHome() {
      this.$router.push("/");
    }
  }
};
</script>

<style lang="less" scoped>
.error-wrapper {
  padding-top: 80px;
  text-align: center;
  .text {
    font-size: 14px;
    color: rgba(45, 48, 59, 0.4);
    line-height: 20px;
    margin-bottom: 24px;
  }
}
</style>
