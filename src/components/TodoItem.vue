<!--
 * @Author: your name
 * @Date: 2021-11-25 11:19:48
 * @LastEditTime: 2021-11-26 02:35:49
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: /Vue-learn-related/src/components/TodoItem.vue
-->
<template>
<ul>

  <li v-for="item in todolist" :key="item.id"> 
      
      <div>
        <input type="checkbox" />
        <span>{{item.title}}</span>
      </div>
      <div>
        <button>remove</button>
      </div>
    </li>
</ul>
</template>

<script>
export default {    
    name: 'TodoItem',
    props:['todolist']
}
</script>

<style>

</style>