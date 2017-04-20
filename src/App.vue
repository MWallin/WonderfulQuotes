<template>
  <div>

    <appHeader></appHeader>

    <appCounter></appCounter>

    <appNew></appNew>

    <appQuotes></appQuotes>

  </div>
</template>



<script>
  import Header from "./components/Header.vue"
  import Counter from "./components/Counter.vue"
  import New from "./components/New.vue"
  import Quotes from "./components/Quotes.vue"

  export default {
    components: {
      appHeader : Header,
      appCounter: Counter,
      appNew    : New,
      appQuotes : Quotes
    }
  }

</script>



<style scoped>

</style>
