<template>
  <div>
    <div class="columns">
      <div class="column is-10 is-offset-1">
        <div class="columns is-multiline quotes">


          <appQuote
            v-for="quote in quotes"
            :likes="quote.likes"
          >

            <span slot="text">
              {{ quote.text }}
            </span>

          </appQuote>


        </div>
      </div>
    </div>
  </div>
</template>



<script>
import Quote from "./Quote.vue"
import { quoteBus } from "../main.js"

export default {

  components: {
    appQuote: Quote
  },

  data: function() {
    return {

      quotes: [
        {
          text : "There are two hard things in computer science: cache invalidation, naming things, and off-by-one errors.",
          likes: 3
        }
      ]

    }
  },

  created() {
    quoteBus.$on( "newQuote", ( text ) => {

      this.quotes.push({
        text,
        likes: 0
      })

    })



  }



}

</script>



<style scoped>
</style>
