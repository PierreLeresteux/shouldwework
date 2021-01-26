<template>
    <div class="why">{{ why }}</div>
</template>

<style>
.why {
    font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
    display: block;
    font-weight: 300;
    font-size: 40px;
    color: #526488;
    letter-spacing: 1px;
}
</style>

<script>
export default {
  data() {
        //const date = new Date(2021,0,23);  
        const date = new Date();
        var day = date.getDate();
        var why = "Because !";

        if (date.getDay() == 6 ||  date.getDay() == 0) {
            why = "Because it's the weekend!";
        } else {
            if (day % 2 != 0) {
                why = "Because it's an odd day!";
            }else {
                why = "Because it's an even day!";
            }
        }
        //const funfact = $http.get('https://api.nuxtjs.dev/mountains')
        
        //http://numbersapi.com/1/25/date

        return { why:why, funfact:"" };
    },
}
</script>