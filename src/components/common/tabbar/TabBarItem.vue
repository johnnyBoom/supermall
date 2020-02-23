<!--  -->
<template>
    <div class="tab-bar-item" @click="itemClick">
        <div v-if="!actived"><slot name="item-icon"></slot></div>
        <div v-else><slot name="item-icon-active"></slot></div>
        <div :class="{active:actived}"><slot name="item-text"></slot></div>
    </div>
</template>

<script>
export default {
name:'TabBarItem',
props:{
    path:String
},
data() {
return {
    // actived: false
}
},
methods: {
    itemClick(){
        this.$router.replace(this.path)
    }
},
computed: {
    actived(){
        return this.$route.path.indexOf(this.path) !== -1
    }
},
//生命周期 - 创建完成（访问当前this实例）
created() {

},
//生命周期 - 挂载完成（访问DOM元素）
mounted() {

}
}
</script>
<style scoped>
/* @import url(); 引入css类 */
.tab-bar-item{
  flex: 1;
  text-align: center;
  height: 49px;
}
.tab-bar-item img{
    width: 24px;
    height: 24px;
    margin-top: 3px;
    vertical-align: middle;
    margin-bottom: 2px;
}
.active{
    color: black;
}
</style>