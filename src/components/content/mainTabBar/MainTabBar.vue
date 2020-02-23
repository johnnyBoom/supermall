<!--  -->
<template>
<div id="mainTabBar">
    <tab-bar>
      <tab-bar-item path="/home">
        <img slot="item-icon" src="~assets/img/tabbar/首页.svg" alt="首页">
        <img slot="item-icon-active" src="~assets/img/tabbar/首页-fill.svg" alt="首页">
        <div slot="item-text">首页</div>
      </tab-bar-item>
      <tab-bar-item path="/category">
        <img slot="item-icon" src="~assets/img/tabbar/搜索类目.svg" alt="分类">
        <img slot="item-icon-active" src="~assets/img/tabbar/搜索类目-fill.svg" alt="分类">
        <div slot="item-text">分类</div>
      </tab-bar-item>
      <tab-bar-item path="/cast">
        <img slot="item-icon" src="~assets/img/tabbar/购物车.svg" alt="购物车">
        <img slot="item-icon-active" src="~assets/img/tabbar/购物车-fill.svg" alt="购物车">
        <div slot="item-text">购物车</div>
      </tab-bar-item>
      <tab-bar-item path="/profile">
        <img slot="item-icon" src="~assets/img/tabbar/我的.svg" alt="我的">
        <img slot="item-icon-active" src="~assets/img/tabbar/我的-fill.svg" alt="我的">
        <div slot="item-text">我的</div>
      </tab-bar-item>
    </tab-bar>
  </div>
</template>

<script>
import TabBar from "components/common/tabbar/TabBar"
import TabBarItem from "components/common/tabbar/TabBarItem"
export default {
  name: 'MainTabBar',
  components: {
    TabBar,
    TabBarItem
  }
}
</script>
<style scoped>
/* @import url(); 引入css类 */

</style>