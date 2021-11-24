<!--
 * @Author: your name
 * @Date: 2021-11-24 22:14:39
 * @LastEditTime: 2021-11-25 05:47:37
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: /Vue-learn-related/src/App.vue
-->
<template>
  <div>
    <h1>Todo List</h1>
    <div class="header">
      <input
        type="text"
        placeholder="Please input backlog, press Enter to confirm"
      />
    </div>
    <ol class="main">
      <li>
        <div>
            <input type="checkbox" />
            <span>sleep</span>
        </div>
        <div>
        <button>remove</button>

        </div>

      </li>
      <li>
        <div>
            <input type="checkbox" />
            <span>eat rice</span>
        </div>
        <div>
        <button>remove</button>

        </div>

      </li>
      <li>
        <div>
            <input type="checkbox" />
            <span>coding</span>
        </div>
        <div>
        <button>remove</button>

        </div>

      </li>
     
    </ol>
    <div class="footer">
        <div>
            <input type="checkbox" />
            <span>selected 2</span>
            /
            <span>all 3</span>

        </div>
      <button>delete selected</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
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

    /* main style */
    .main{
        margin-top: 20px;
        width: 100%;
        box-sizing: border-box;
    }
    .main li{
        margin-left: 5px;
        display: flex;
        justify-content:space-between;
        margin-right: 5px;
        height: 30px;
        
    }

    /* footer style */
    .footer{
        margin-top: 15px;
        margin-left: 5px;
        display: flex;
        justify-content: space-between;
    }
    .footer button{
        margin-right: 5px;
    }


</style>