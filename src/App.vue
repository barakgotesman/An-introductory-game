<template>
  <div id="app">
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <CardQuestion @click="test()" />
    <p @click="test">{{ myCards }}</p>
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue';
import CardQuestion from './components/CardQuestion.vue';

export default {
  components: {
    CardQuestion
  },
  setup(){
    const name= 'App',
    const myCards = ref([]),
    const myCardsViewd = [],
    function test() {
      console.log('test',myCards);
      myCards.push("test");
    }
    return {name,myCards,myCardsViewd, test}
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
