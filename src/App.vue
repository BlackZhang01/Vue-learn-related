<!--
 * @Author: your name
 * @Date: 2021-11-24 22:14:39
 * @LastEditTime: 2021-11-24 23:15:14
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: /Vue-learn-related/src/App.vue
-->
<template>
  <div>
    <h1>Todo List</h1>
    <input type="text" placeholder="Please input backlog, press Enter to confirm">
    <ul>
      <li>
        <input type="checkbox">
        sleep
      </li>
      <li>
        <input type="checkbox">
        eat rice
      </li>
      <li>
        <input type="checkbox">
        coding
      </li>
    </ul>
    <div>
      <input type="checkbox">
      <span>selected 2</span>
      /
      <span>all 3</span>
      <button>delete selected</button>
    </div>
  </div>
</template>

<script>
export default {  
  name:'App'

}
</script>

<style>

</style>