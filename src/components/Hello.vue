<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <v-alert type="success" message="ceshi"></v-alert>
  </div>
</template>

<script>

import vAlert from '../../components/alert'

export default {
  data () {
    return {
      alert: 'Hello World!'
    }
  },
  components: {
    vAlert
  }
}
</script>

<style scoped>
h1 {
  color: #42b983;
}
</style>
