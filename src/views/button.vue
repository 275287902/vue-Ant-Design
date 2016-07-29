<template lang="html">

  <div>

    <section class="markdown">
      <h1>Button 按钮</h1>
      <p>
        按钮用于开始一个即时操作。
      </p>
      <h2>何时使用</h2>
      <ul>
        <p>
          标记了一个（或封装一组）操作命令，响应用户点击行为，触发相应的业务逻辑。
        </p>
      </ul>
      <h2>组件演示</h2>
    </section>

    <div class="ant-row" style="margin-left: -8px; margin-right: -8px;">

      <div class="ant-col-lg-12 code-boxes-col-2-1">

        <code-box
          title="基础"
          describe="简单的徽章展示。"
          code='<v-badge :count="30"><a href="#" class="head-example"></a></v-badge>'
        >
          <v-button type='primary'>Primary</v-button>
          <v-button>default</v-button>
          <v-button type='ghost'>Ghost</v-button>
          <v-button type='dashed'>Dashed</v-button>
        </code-box>

      </div>

      <div class="ant-col-lg-12 code-boxes-col-2-1">

        <code-box
          title="基础"
          describe="简单的徽章展示。"
          code=''
        >
          <v-button type='primary' shape="circle" icon="search"></v-button>
          <v-Button type="primary" icon="search"><span>搜索</span></v-Button>
          <br />
          <br />
          <v-Button type="ghost" shape="circle-outline" icon="search" /></v-button>
          <v-Button type="ghost" icon="search"><span>搜索</span></v-Button>
        </code-box>

      </div>
    </div>


    <api-table
      :apis='apis'
    ></api-table>

  </div>

</template>

<script>

import vButton from '../../components/button'
import codeBox from '../components/codeBox'
import apiTable from '../components/apiTable'

export default {
  data: function () {
    return {
      apis: [{
          parameter: 'type',
          explain: '必选参数，指定警告提示的样式，有四种选择 success、info、warning、error',
          type: 'String',
          default: 'info'
        },{
          parameter: 'closable',
          explain: '可选参数，默认不显示关闭按钮',
          type: 'Boolean',
          default: 'false'
        },{
          parameter: 'closeText',
          explain: '可选参数，自定义关闭按钮',
          type: 'String',
          default: '无'
        },{
          parameter: 'message',
          explain: '必选参数，警告提示内容',
          type: 'String',
          default: '无'
        },{
          parameter: 'description',
          explain: '可选参数，警告提示的辅助性文字介绍',
          type: 'String',
          default: '无'
        },{
          parameter: 'onClose',
          explain: '可选参数，关闭时触发的回调函数',
          type: 'Function',
          default: '无'
        },{
          parameter: 'showIcon',
          explain: '可选参数，是否显示辅助图标',
          type: 'Boolean',
          default: 'false'
        },{
          parameter: 'closed',
          explain: '可选参数，控制组件隐藏显示，默认显示',
          type: 'Boolean',
          default: 'false'
        }
      ]
    }
  },
  components: {
    vButton,
    codeBox,
    apiTable
  }
}
</script>

<style lang="less">
</style>
