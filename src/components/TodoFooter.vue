<!--
 * @Author: your name
 * @Date: 2021-11-25 11:19:23
 * @LastEditTime: 2021-11-25 11:25:36
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: /Vue-learn-related/src/components/TodoFooter.vue
-->
<template>
  <div class="footer">
        <div>
            <input type="checkbox" />
            <span>selected 2</span>
            /
            <span>all 3</span>

        </div>
      <button>delete selected</button>
    </div>
</template>

<script>
export default {
    name: 'TodoFooter'
}
</script>

<style scoped>
    /* footer style */
    .footer{
        width: 400px;
        margin-top: 15px;
        margin-left: 5px;
        display: flex;
        justify-content: space-between;
    }
    .footer button{
        margin-right: 5px;
    }
</style>