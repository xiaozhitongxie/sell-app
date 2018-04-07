<template>
  <div>
   <vheader></vheader>
    <div class="tab">
      <div class="tab-item">
        <a v-link="{path:'/goods'}">商品</a>
       </div>
      <div class="tab-item">
        <a v-link="{path:'/ratings'}">评论</a>
      </div>
      <div class="tab-item">
        <a v-link="{path:'/seller'}">商家</a>
      </div>
    </div>
    <router-view></router-view>
  </div>
</template>

<script>
import vheader from 'components/vheader/vheader'
export default {
  components: {
    vheader
  }
}
</script>

<style scoped lang="stylus" rel="stylesheet.stylus">
    .tab
      display:flex
      width:100%
      height:40px
      line-height:40px
      .tab-item
        flex:1
        text-align:center
</style>
