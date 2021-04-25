<template>
  <div id="app">
    <Header msg="Posts"/>
      <Content v-bind:todos="todos"/>
  </div>
</template>

<script>
import Header from './components/Header'
import Content from './components/Content'

export default {
  name: 'App',
  data() {
    return {
      todos: [
        {
          id: 1,
          title: "delectus aut autem",
          completed: false
        },
        {
          id: 2,
          title: "quis ut nam facilis et officia qui",
          completed: false
        },
        {
          id: 3,
          title: "fugiat veniam minus",
          completed: false
        },
        {
          id: 4,
          title: "et porro tempora",
          completed: true
        }
      ]
    }
  },
  components: {
    Header,
    Content
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

  ul {
    list-style: none;
    text-align: left;
    padding: 0;
    margin: 0;
  }
</style>
