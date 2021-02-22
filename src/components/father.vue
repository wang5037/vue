<template>
  <div id="father" style="background:yellow;width:500px;height:400px">
      <h1>我是父组件的背景</h1>
        <Chilid>
            <div slot="chaCao1" style="border:1px solid blue">我是具名插槽blue边框1</div>
            <div slot="chaCao2" slot-scope='jie' style="border:1px solid pink">
                我是传值的作用域插槽<br>
            <span v-for="(item,index) in jie.chuan" :key="index">姓名：{{item.name}} 性别：{{item.sex}} 年龄：{{item.age}}</span>
    </div> 
            <div style="border:1px solid #cccccc">我是匿名插槽</div>
        </Chilid>
  </div>
</template>

<script>

import Chilid from "../components/chilid.vue";
export default {
  components: { Chilid },
};
</script>

<style>
</style>