<template>
    <h2 class="subtitle">
        The answer is NO
        <div v-if="odd">Because it's an odd day !</div>
        <div v-else="odd">Because it's an even day !</div>
    </h2>
</template>

<style>
    .subtitle {
    font-weight: 300;
    font-size: 42px;
    color: #526488;
    word-spacing: 5px;
    padding-bottom: 15px;
    }

</style>

<script>
export default {
  data() {
        var day = new Date().getDate();
        return {
            odd: day % 2 != 0
        }
    },
    
}
</script>