<template lang="html">

  <button type="button" :class="['ant-btn', type, size, shape]" :class="{'ant-btn-loading': loading}">
    <i class="anticon anticon-loading" v-if="loading"></i>
    <i class="anticon anticon-{{icon}}" v-if="icon"></i>
    <slot></slot>
  </button>

</template>
type
<script>
export default {
  props: {
    type: {
      type: String,
      coerce: function (val) {
        return `ant-btn-${val}`
      }
    },
    icon: String,
    shape: {
      type: String,
      coerce: function (val) {
        return `ant-btn-${val}`
      }
    },
    size: String,
    loading: {
      type: Boolean,
      default: false
    }
  },
  data: function () {
    return {
    }
  },
  ready: function () {},
  attached: function () {},
  methods: {},
  components: {}
}
</script>

<style lang="css">
</style>
