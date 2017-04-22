<template>

  <div class="column is-one-quarter quote">
    <div class="card">

      <div class="card-content">
        <div class="content">

          <slot name="text"></slot>

        </div>
      </div>

      <footer class="card-footer">

        <a class="card-footer-item" @click="likeQuote">
          <span class="icon is-medium">
            <i class="fa fa-thumbs-o-up"></i>
          </span>
          <span>

            {{ likes }}

          </span>
        </a>

        <a class="card-footer-item" @click="deleteQuote">Delete</a>
      </footer>

    </div>
  </div>

</template>



<script>

export default {

  props: {
    likes: {
      type: Number
    }
  },

  methods: {

    likeQuote() {
      this.likes++
    },

    deleteQuote() {
      console.log( "Deleted a quote" )
    }

  }

}

</script>



<style scoped>

.icon {
  margin-right: 10px;
}

.card-footer {
  font-size: 25px;
}

.quotes {
  padding: 12px;
}

.quote {
  font-family: 'Satisfy', cursive;
  font-size: 30px;
  display: flex;
  justify-content: center;
  align-items: center;
}

</style>
