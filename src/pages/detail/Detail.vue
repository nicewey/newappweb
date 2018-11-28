<template>
  <div>
    <detail-banner></detail-banner>
    <detail-header></detail-header>
    <detail-list :list="list"></detail-list>
    <div class="content"></div>
  </div>
</template>

<script>
import DetailBanner from './components/Banner'
import DetailHeader from './components/Header'
import DetailList from './components/List'
export default {
  name: 'Detail',
  components: {
    DetailList,
    DetailBanner,
    DetailHeader
  },
  data () {
    return {
      list: [{
        title: '大师赛',
        children: [{
          title: 'asdqs',
          children: [{
            title: 'yyyyy'
          }]
        }, {
          title: 'sdfbh'
        }]
      }, {
        title: '阿萨大'
      }, {
        title: 'asd'
      }, {
        title: 'afed'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .content
    height: 50rem
</style>
