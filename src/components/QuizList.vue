<template>
  <div>
  <quiz v-for="quiz in quizzes" v-bind:quiz="quiz" :key="quiz.id" class="ui centered card"></quiz>
        
    </div>
  </div>
</template>

<script>
import Quiz from './Quiz';
export default {

  props:['quizzes'],
  components: {
    Quiz
  }

  }
</script>