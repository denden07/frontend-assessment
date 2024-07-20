<template>
  <div id="app">
   <ExerciseView></ExerciseView>
  </div>
</template>

<script>
import ExerciseView from './views/ExerciseView/ExerciseView.vue'

export default {
  name: 'App',
  components: {
    ExerciseView
  }
}
</script>

<style src='./assets/styles/css/main.min.css'></style>
