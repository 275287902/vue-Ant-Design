<template lang="html">

  <div class="main-wrapper">
    <div class="ant-row">
      <div class="ant-col-xs-24 ant-col-sm-24 ant-col-md-6 ant-col-lg-4">
        <v-menu class="aside-container" mode="inline">
          <menu-item>
            <a href="/">快速上手</a>
          </menu-item>
          <menu-item>
            <a href="/">安装</a>
          </menu-item>
          <menu-item>
            <a href="/">更新日志</a>
          </menu-item>
          <sub-menu title="Baseic">
            <menu-item v-link="{ name: 'button', activeClass: 'ant-menu-item-selected' }">
              Button 按钮
            </menu-item>
          </sub-menu>
          <sub-menu title="Components">
            <menu-item v-link="{ name: 'alert', activeClass: 'ant-menu-item-selected' }">
              Alert 警告提醒
            </menu-item>
            <menu-item v-link="{ name: 'alert', activeClass: 'ant-menu-item-selected' }">
              Alert 警告提醒
            </menu-item>
            <menu-item v-link="{ name: 'badge', activeClass: 'ant-menu-item-selected' }">
              Badge 徽标数
            </menu-item>
            <menu-item v-link="{ name: 'card', activeClass: 'ant-menu-item-selected' }">
              Card 卡片
            </menu-item>
            <menu-item v-link="{ name: 'collapse', activeClass: 'ant-menu-item-selected' }">
              Collapse 折叠面板
            </menu-item>
            <menu-item v-link="{ name: 'dropdown', activeClass: 'ant-menu-item-selected' }">
              Dropdown 下拉菜单
            </menu-item>
          </sub-menu>
        </v-menu>
      </div>
      <div class="main-container ant-col-xs-24 ant-col-sm-24 ant-col-md-18 ant-col-lg-20">
        <router-view keep-alive></router-view>
      </div>
    </div>
  </div>

</template>

<script>

import vMenu from '../../components/menu'
let menuItem = vMenu.Item
let subMenu = vMenu.subMenu

export default {
  data: function () {
    return {
    }
  },
  computed: {},
  ready: function () {},
  attached: function () {},
  methods: {},
  components: {
    vMenu,
    menuItem,
    subMenu
  }
}
</script>

<style lang="less">

.main-wrapper {
    width: 96%;
    margin: 0 auto;
    border-radius: 6px;
    padding: 24px 0 0;
    margin-bottom: 24px;
    background-color: #fff;
    overflow: hidden;
    position: relative;
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

.aside-container {
    padding-bottom: 50px;
}

.aside-container .ant-menu-item a, .aside-container .ant-menu-submenu-title span, .aside-container>.ant-menu-item {
    font-size: 14px;
    text-overflow: ellipsis;
    overflow: hidden;
}

</style>
