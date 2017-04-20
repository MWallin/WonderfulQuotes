<template>
  <div>
    <div class="columns">
      <div class="column is-10 is-offset-1">

        <div class="columns is-multiline quotes">



          <div class="column is-one-quarter quote">
<div class="card">
  <div class="card-content">
    <p class="title">
      “There are two hard things in computer science: cache invalidation, naming things, and off-by-one errors.”
    </p>
  </div>
</div>
          </div>


          <div class="column is-one-quarter quote">
<div class="card">
  <div class="card-content">
    <p class="title">
      This is a really amazing and inspiring quote!
    </p>
  </div>
</div>
          </div>









        </div>


        <section class="delete-info">
          <h5>
            Click on a qoute to delete it!
          </h5>
        </section>

      </div>
    </div>
  </div>
</template>



<script>
</script>



<style scoped>

  .quotes {
    padding: 12px;
  }

  .quote {
    font-family: 'Yellowtail', cursive;
    font-size: 35px;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .delete-info {
    background-color: #00D1B2;
    height: 45px;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
    font-size: 18px;
  }

</style>
