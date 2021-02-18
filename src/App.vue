<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <MyName name="My Name is Riwandi" age="25"/>
  <p>my favourite game is:</p>
  <ul>
    <li v-for="list in lists" :key="list.id">{{ list.name }}</li>
  </ul>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import MyName from './components/MyName'

export default {
  name: 'App',
  components: {
    HelloWorld,
    MyName
  },
  data() {
    return {
      lists: [
        {
          id: 1,
          name: 'Dota 2',
        },
        {
          id: 2,
          name: 'RE7'
        }
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

li {
  list-style-type: none;
}
</style>
