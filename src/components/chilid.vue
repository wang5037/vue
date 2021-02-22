<template>
  <div id="chilid" style="border:1px solid red;height:400px">
      <h3>我是子组件</h3>
      <slot name="chaCao1"></slot>
      <slot name="chaCao2" :chuan="arr"></slot>

      <slot></slot>
  </div>
</template>

<script>
export default {
    data(){
        return{
            arr:[
        {"name":"张三","sex":"男","age":18},
        {"name":"李四","sex":"男","age":28},
        ]
    }}
}
</script>

<style>

</style>