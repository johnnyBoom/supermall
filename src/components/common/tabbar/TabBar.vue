<!--  -->
<template>
   <div id="tab-bar">
    <slot></slot>
   </div>
</template>

<script>
export default {
name:"TabBar",
data() {
return {

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
 
#tab-bar{
  display: flex;
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #f6f6f6;
  box-shadow: 0 -3px 1px rgba(100, 100, 100, 0.1);
}
</style>