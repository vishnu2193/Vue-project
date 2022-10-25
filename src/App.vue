<template>
  <h1>{{name }}</h1>
  <!-- using if statemment hide/show the child component -->
  <div v-if="showChild">
<!-- sending props below -->
<!-- another way to send props with binding ex:'Vis' -->
  <ChildVue :Vis='Vis' Text="Another props"/>
  </div>
  <!-- calling method by onclick -->
  <button @click="ChildOpen">ShowChildBtn</button>
</template>

<script>
import ChildVue from './components/Child.vue';
export default {
  name: 'App',
  components:{ChildVue},
  data() {
    return {
      name: 'Vishnu',
      Vis:'Hello prop',
      // below is flag to show/hide child component
      showChild:false
    };
  },
  methods:{
    // below method will show/hide child component
    ChildOpen(){
      this.showChild= !this.showChild;
    }
  }
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
