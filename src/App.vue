<template>
  <div id="app">
    <v-alert type="success" message="成功提示的文案"></v-alert>
    <v-alert type="info" message="消息提示的文案"></v-alert>
    <v-alert type="warning" message="警告提示的文案"></v-alert>
    <v-alert type="error" message="错误提示的文案"></v-alert>
  </div>
</template>

<script>

import vAlert from '../components/alert'

export default {
  components: {
    vAlert
  }
}
</script>

<style lang="less">

@import "../style/index.less";

#app {
  margin-top: 60px;
  color: #2c3e50;
  max-width: 600px;
}

#app a {
  color: #42b983;
  text-decoration: none;
}

.logo {
  width: 100px;
  height: 100px
}
</style>
