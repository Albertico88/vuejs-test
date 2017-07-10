<template>
  <div class="Contact">
    <div class="container">
      <section class="section">

        <h1 class="title">Contact Us</h1>
        <h2 class="subtitle is-4">Lorem ipsum dolor sit amet, consectetur adipisicing elit.</h2>

        <div class="columns">
          <div class="column is-half">
            <div class="card">
              <div class="card-content">
                <p class="title">Email us!</p>
                <p class="answer">Send us an email to test@testingvue.com</p>
              </div>
            </div>
          </div>

          <div class="column is-half">
            <div class="card">
              <div class="card-content is-large">
                <p class="title">Call us!</p>
                <p class="answer">Operators available M-F 8am-6pm <br><strong>(787)789-1234</strong></p>
              </div>
            </div>
          </div>
        </div>

      </section>
    </div>
  </div>
</template>



<script>


</script>





<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>
@import "../mediaQuery"

.pd
  padding: 2.5em 0 1.5em 0

.answer
  margin-top: 10px !important
  color: gray

.columns
  flex-wrap: wrap


</style>
