<template>
<div>
  <h1>{{title}}</h1>
  <Modal header="Sign up for the Giveaway"/>
</div>
</template>

<script>
import Modal from './components/Modal'

export default {
  name: 'App',
  components: {Modal},
  data() {
    return {
      title: 'My first template'
    }
  },
  
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
h1 {
  border-bottom: 1px solid #ddd;
  display: inline-block;
  padding-bottom: 10px;
}
</style>
