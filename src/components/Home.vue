
<template>

  <div class="home">

    <section class="hero">
      <div class="hero-body">
        <div class="container">
          <h1 class="title">{{ heading }}</h1>
          <div class="is-two-thirds column is-paddingless">
            <h2 class="subtitle">{{ subheading }}</h2>
          </div>
          <a class="button is-large is-primary" id="learn" href="#/faq">Learn more</a>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="container">
        <div class="columns pd is-desktop">
          <div class="column is-1 has-text-centered">
            <i class="fa fa-cog is-primary"></i>
          </div>
          <div class="column is-one-third-desktop">
            <p class="title">
              <strong>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</strong>
            </p>
          </div>
          <div class="column">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt.
            </p>
          </div>
        </div>
      </div>


    <div class="columns pd">

      <div class="column">
        <div class="card">
          <div class="card-content">
            <p class="title">
              “You only live once, but if you do it right, once is enough.”
            </p>
            <br>
            <p class="subtitle">- Mae West
            </p>
          </div>
        </div>
      </div>

      <div class="column">
        <div class="card">
          <div class="card-content">
            <p class="title">
              “A room without books is like a body without a soul.”
            </p>
            <br>
            <p class="subtitle"> -  Marcus Tullius Cicero
            </p>
          </div>
        </div>
      </div>

      <div class="column">
        <div class="card">
          <div class="card-content">
            <p class="title">
              “In three words I can sum up everything I've learned about life: it goes on.”
            </p>
            <br>
            <p class="subtitle"> - Robert Frost
            </p>
          </div>
        </div>
      </div>

    </div>
  </section>
  </div>

</template>



<script>

export default {
  name: 'home',
  data (){
    return {
      heading: 'Large call to action goes here',
      subheading: 'Subheading to the call to action goes in here to detail a bit more of information. This is just some dummy text to lengthen this up a bit until it takes up 2/3 of the width.'
    }
  }
}

</script>



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>
@import "../mediaQuery"


.hero
  background: url('../assets/beach.jpg')
  background-size: cover
  background-position: 0 59%

  .title
    +mobile
      font-weight: bold
    +tablet
      font-size: 2.5rem
    +desktop
      font-size: 4rem
      margin-top: 2rem

h2
  margin: 1.5rem 0 2rem 0 !important
  color: black

.fa-cog
  font-size: 40px

#learn
  +desktop
    margin-bottom: 2rem

.pd
  +tablet
    padding: 2em 0

</style>
