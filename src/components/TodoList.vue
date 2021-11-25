<!--
 * @Author: your name
 * @Date: 2021-11-25 11:19:11
 * @LastEditTime: 2021-11-26 05:38:08
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: /Vue-learn-related/src/components/TodoList.vue
-->
<template>
  <div class="main">
    <TodoItem :removeTodo="removeTodo" :selectTodo="selectTodo" :todolist="todolist" />
    
  </div>
</template>

<script>
import TodoItem from './TodoItem'


export default {
  name: "TodoList",
  props:['todolist','selectTodo','removeTodo'],
  components: {
    TodoItem
  }
};
</script>

<style>
/* main style */
.main {
  margin-top: 20px;
  width: 400px;
  box-sizing: border-box;
}
.main li {
  margin-left: 5px;
  display: flex;
  justify-content: space-between;
  margin-right: 5px;
  height: 30px;
}
.main button{
  display: none;
}
.main li:hover {
  background-color: gray;
}
.main li:hover button{
  display: inline-block;
}
</style>