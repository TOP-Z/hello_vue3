<!--
 * @Description: 
 * @Author: 振顺
 * @Date: 2024-01-02 16:44:48
 * @LastEditTime: 2024-01-02 17:09:13
 * @LastEditors: 振顺
-->
<template>
  <div class="app">
    <h1>你好啊！</h1>
    <Person />
  </div>
</template>

<script lang="ts">
import Person from "./components/Preson.vue";
export default {
  name: "App", //组件名
  components: {
    Person,
  },
};
</script>
<style>
.app {
  background-color: #ddd;
  box-shadow: 0 0 10px;
  border-radius: 10px;
  padding: 20px;
}
</style>
