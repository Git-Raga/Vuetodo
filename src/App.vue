<template>
  
  <div id="app"> 
    <div class="todo_wrapper">
      <div class="todo_list">
        <TodoList />
          <div class="btn-container">
             <div class="create-btn">
              Create ToDo
             </div>  
           </div>
      </div>
    
    </div>

 

  
  </div>
</template>

<script>

import TodoList from './components/TodoList.vue'
// using import we get the component to App.vue page and then
//using export we put that in to the above template
//for understanding
export default {
    name: 'app',
    components: {
      TodoList
  
  }
}


</script>

<style lang="scss">//npm install --save sass-loader node-sass
//create a webpack.config.js file and paste the contents from 
//https://vue-loader.vuejs.org/guide/pre-processors.html#sass-vs-scss
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}

.btn-container{
  
    background-color: #edcded;
    border-radius: 5px;
     
}
.create-btn{
    font-size: 20px;
    padding: 10px;
    border-radius: 5px;
    background-color: #795899;
    color: white;
    font-weight: bold;
    text-align: center;
  }

 .todo{
   &_wrapper{
    display: flex;
    justify-content: center;
    width: 100%;
    
  }
  &_list{
        display: flex;
        flex-direction: column;
        width: 400px;
        min-height: 200px;
        background-color: #ededed;
        border-radius: 5px;
        padding:15px;
     }
   
 }

 
</style>

// TODO: Create Array for Todolist
// TODO: Sync with GITHUB and Push
