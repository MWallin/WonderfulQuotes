<template>
  <div class="container">
    <div class="columns">
      <div class="column is-half is-offset-one-quarter">


        <div class="field">
          <!--<label class="label">New quote goes here...</label>-->
          <p class="control">
            <textarea class="textarea" v-model="text"></textarea>
          </p>
        </div>

        <div class="has-text-centered">
          <button class="button is-primary" @click="addQuote">
            <span class="icon">
              <i class="fa fa-pencil"></i>
            </span>
            <span>Click here to add new quote</span>
          </button>
        </div>


      </div>
    </div>
  </div>
</template>



<script>
import { quoteBus } from "../main.js"

export default {

  data: function() {
    return {
      text  : "",
      quotes: 1
    }
  },

  methods: {

    addQuote() {

      // If 10, then alert

      if ( this.text.length > 0 ) {

        quoteBus.$emit( "newQuote", this.text )

        this.text = ""

        this.quotes++

      }


    }


  }

}


</script>



<style scoped>



</style>
