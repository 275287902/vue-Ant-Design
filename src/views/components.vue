<template lang="html">

  <div class="main-wrapper">
    <div class="ant-row">
      <div class="ant-col-lg-4"></div>
      <div class="main-container ant-col-lg-20">
        <router-view keep-alive></router-view>
      </div>
    </div>
  </div>

</template>

<script>
export default {
  data: function () {
    return {
    }
  },
  computed: {},
  ready: function () {},
  attached: function () {},
  methods: {},
  components: {}
}
</script>

<style lang="less">

.main-wrapper {
    width: 1140px;
    margin: 0 auto;
    border-radius: 6px;
    padding: 24px 0 0;
    margin-bottom: 24px;
}

.main-container {
    padding: 0 6% 120px 4%;
    margin-left: -1px;
    min-height: 500px;
    border-left: 1px solid #e9e9e9;
}

.markdown{
  color: #666;
  font-size: 14px;
  line-height: 1.8;

  h1 {
      color: #404040;
      font-weight: 500;
      line-height: 40px;
      margin-bottom: 24px;
      margin-top: 8px;
      font-size: 28px;
      font-family: lato,Helvetica Neue,Helvetica,PingFang SC,Hiragino Sans GB,Microsoft YaHei,Arial,sans-serif;
  }

  p, pre {
      margin: 1em 0;
  }

  h2 {
      font-size: 22px;
  }

  h2, h3,  h4,  h5,  h6 {
      color: #404040;
      font-family: lato,Helvetica Neue,Helvetica,PingFang SC,Hiragino Sans GB,Microsoft YaHei,Arial,sans-serif;
      margin: 1.6em 0 .6em;
      font-weight: 500;
      clear: both;
  }
}

.code-boxes-col-2-1{
  display: inline-block;
  vertical-align: top;
  padding: 0 8px;
}

</style>
