<template>
  <d2-container :filename="filename" type="ghost">
    <d2-module-index-banner slot="header" v-bind="banner"/>
    <d2-module-index-menu :menu="menu"/>
  </d2-container>
</template>

<script>
import menu from '@/menu/modules/demo-filters'
export default {
  data () {
    return {
      filename: __filename,
      menu,
      banner: {
        title: 'FILTERS',
        subTitle: '内置过滤器'
      }
    }
  }
}
</script>
