<template>
  <div class="container">
    <div>
      <logo />
      <question />
      <h2 class="subtitle">
        The answer is NO
      </h2>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Question from '~/components/Question.vue'

export default {
  components: {
    Logo,
    Question
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}



.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

</style>
