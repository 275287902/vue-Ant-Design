<template lang="html">

  <v-alert type="success" message="成功提示的文案"></v-alert>
  <v-alert type="info" message="消息提示的文案"></v-alert>
  <v-alert type="warning" message="警告提示的文案"></v-alert>
  <v-alert type="error" message="错误提示的文案"></v-alert>

</template>

<script>

import vAlert from '../components/alert'

export default {
  data: function () {
    return {
    }
  },
  components: {
    vAlert
  }
}
</script>

<style lang="css">
</style>
