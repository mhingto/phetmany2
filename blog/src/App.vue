<template>
  <div id="app">
        <EmployeeList />

        <hr />

        <PostComponent />
  </div>
</template>

<script>
import EmployeeList from './components/EmployeeList';
import PostComponent from './components/PostComponent';
export default {
  name: 'App',
  components: {
    EmployeeList,
    PostComponent
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
</style>
