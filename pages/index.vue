<template>
  <div class="container">
    <div>
      <img src="https://i.imgur.com/HXucnOl.gif" />
      <question />
      <no />
      <why />
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Question from '~/components/Question.vue'
import No from '~/components/No.vue'
import Why from '~/components/Why.vue'

export default {
  components: {
    Logo,
    Question,
    No,
    Why,
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
