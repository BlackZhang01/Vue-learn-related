<!--
 * @Author: your name
 * @Date: 2021-11-24 22:14:39
 * @LastEditTime: 2021-11-26 02:48:24
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: /Vue-learn-related/src/App.vue
-->
<template>
  <div id="app">
    <h1>Todo List</h1>
    <TodoHeader :addItem="addItem" />
    <TodoList :todolist="todolist"/>
    <TodoFooter/>
  </div>
</template>


<script>

import TodoHeader from './components/TodoHeader'
import TodoList from './components/TodoList'
import TodoFooter from './components/TodoFooter'
import {nanoid} from 'nanoid'

export default {
  name: "App",
  data(){
      return {
          todolist:[
              {id:nanoid(),title:'sleep',isShow:true},
              {id:nanoid(),title:'eat rice',isShow:false},
              {id:nanoid(),title:'write coding',isShow:true}
          ]
      }
  },
  components: {
      TodoHeader,
      TodoList,
      TodoFooter
  },
  methods: {
      addItem(value){
          this.todolist.unshift(value)
      }
  },
};
</script>

<style>
    /* common style */
    body{
        margin: 0;
    }
    button{
        border-style: none;
        background-color: orangered;
        border: solid 1px red;
        border-radius: 3px;
        height: 25px;
    }
    button:hover{
        opacity: 0.7;
    }
    ul,ol,li{
        padding: 0;
        margin: 0;
        list-style: none;
    }

    #app{
        border: solid 1px black;
        padding: 10px;
        margin: 10px;
        width: 400px;
    }

    

    

    


</style>