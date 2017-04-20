<template>
  <section>


<div class="columns">
  <div class="column is-10 is-offset-1">

    <h3 class="title is-3">
      Quotes added
    </h3>

    <div class="counter">
      <div class="current-count has-text-centered">
        1 / 10
      </div>

    </div>

  </div>
</div>


  </section>
</template>



<script>

</script>



<style scoped>

  section {
    margin: 25px 0;
  }

  .counter {
    height: 40px;
    background-color: lightslategray;
    border-radius: 10px;
  }

  .current-count {
    height: 100%;
    width: 10%;
    background-color: #00D1B2;
    display: flex;
    justify-content: center;
    align-items: center;
    border-top-left-radius: 10px;
    border-bottom-left-radius: 10px;
  }

</style>
