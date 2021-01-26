<template>
    <div class="funfact">Funfact of the day: <i>{{ funfact }}</i></div>
</template>

<style>
.funfact {
    font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
    display: block;
    font-weight: 300;
    font-size: 20px;
    color: #526488;
    letter-spacing: 1px;
}
</style>

<script>
import { $fetch } from 'ohmyfetch'

export default {
  data() {
      return {funfact:"" };
  },
  async fetch() {
    this.funfact = await $fetch(
      'http://numbersapi.com/1/25/date'
    )
  }
}
</script>