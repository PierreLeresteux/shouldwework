<template>
  <div class="container">
    <div>
      <logo />
      <question />
      <no />
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Question from '~/components/Question.vue'
import No from '~/components/No.vue'

export default {
  components: {
    Logo,
    Question,
    No,
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

</style>
