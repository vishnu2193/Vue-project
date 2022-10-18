<template>
  <h1>{{name }}</h1>
  <ChildVue/>
</template>

<script>
import ChildVue from './components/Child.vue';
export default {
  name: 'App',
  components:{ChildVue},
  data() {
    return {
      name: 'Vishnu',
    };
  },
};
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
