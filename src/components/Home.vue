
<template>

  <div class="home">

    <section class="hero">
      <div class="hero-body">
        <div class="container">
          <h1 class="title">{{ heading }}</h1>
          <div class="is-two-thirds column is-paddingless">
            <h2 class="subtitle">{{ subheading }}</h2>
          </div>
          <a class="button is-large is-primary" id="learn">Learn more</a>
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
    </section>

    <div class="columns pd">
      <div class="column">
        <div class="card">
          <div class="card-content">
            
          </div>
        </div>
      </div>
    </div>

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


</style>
