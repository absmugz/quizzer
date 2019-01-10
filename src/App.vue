<template>
  <div id="app">
    <quiz-list v-bind:quizzes="quizzes"></quiz-list>
  </div>
</template>

<script>

import QuizList from './components/Quizlist';

export default {
  name: 'App',
  components: {
    QuizList
  },
  data() {
    return {
      quizzes:[{
        title:"Chapter 1",
        description:"This is a sample description.",
        cards: [
          {
            term:"Same Word",
            definition:"Some definition"
          },{
            term:"Same Word",
            definition:"Some definition"
          }
        ]
        },{
        title:"Chapter 2",
        description:"This is a another sample description.",
        cards: []
        }]      
    }
  }
}


</script>

<style>
#app {
  margin-top: 60px;
}
</style>
