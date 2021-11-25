<!--
 * @Author: your name
 * @Date: 2021-11-25 11:18:41
 * @LastEditTime: 2021-11-25 11:24:22
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: /Vue-learn-related/src/components/TodoHeader.vue
-->
<template>
  <div class="header">
      <input
        type="text"
        placeholder="Please input backlog, press Enter to confirm"
      />
    </div>
</template>

<script>
export default {
    name: 'TodoHeader'
}
</script>

<style>
  /* header style */
    .header{
        width: 100%;
        height: 40px;
        line-height: 40px;
        box-sizing: border-box;
    }
    .header input{
        height: 30px;
        width: 300px;
        border-radius: 5px;
        border-style: none;
        margin-left: 5px;
        border: solid 1px black;
    }
</style>