<template>
  <div id="app">

    <!-- Nav Section -->
    <div class="nav has-shadow">
      <div class="container">
        <div class="nav-left">
          <a class="nav-item">Logo</a>
        </div>

      <!-- Hamburger Toggle -->
      <!-- Using Vue directives v- -->
        <span class="nav-toggle" v-on:click="toggleNav" v-bind:class="{ 'is-active': isActive }">
          <span></span>
          <span></span>
          <span></span>
        </span>

        <div class="nav-right nav-menu" v-bind:class="{ 'is-active': isActive }">

        <!-- Links using Vue's router link -->
          <router-link to="/" class="nav-item r-item">Home</router-link>
          <router-link to="/faq" class="nav-item r-item">FAQ</router-link>
          <router-link to="/" class="nav-item r-item">About</router-link>
          <router-link to="/faq" class="nav-item r-item">Contact</router-link>

          <div class="nav-item">
            <p class="control">
              <a class="button is-primary is-outlined">
                <span class="icon">
                  <i class="fa fa-download"></i>
                </span>
                <span>Join Now!</span>
              </a>
            </p>
          </div>

        </div>
      </div>
    </div>


<!-- Components are inserted here -->
    <router-view></router-view>


    <footer class="footer is-primary">
      <div class="container">
        <div class="columns">
          <div class="column">
            <p>
              This is the footer section for the page including some links.
            </p>
          </div>
          <div class="columns has-text-right">
            <a class="icon" href="#"><i class="fa fa-facebook"></i></a>
            <a class="icon" href="#"><i class="fa fa-twitter"></i></a>
          </div>
        </div>
      </div>
    </footer>



  </div>
</template>


<!-- Script -->
<script>
export default {
  name: 'app',
  data: function() {
    return {
      isActive: false
    }
  },
  methods: {
    toggleNav: function() {
      this.isActive = !this.isActive;
    }
  }
}
</script>


<!-- Style -->
<style lang="sass">
/* Import Bulma Css Framework */
@import "../node_modules/bulma/bulma.sass"
@import "mediaQuery"

.nav
  background-color: #383838
  a:hover
    color: gray

.nav-left a
  color: #fff
  font-weight: bold

a.r-item
  color: #C1C1C1
  padding: 0.5rem 1.75rem
  +mobile
    color: gray
    &:hover
      background-color: #F1F1F1

.nav-toggle span
  background-color: #C1C1C1

footer
  background-color: $primary !important
  color: #fff

  .icon
    color: #fff
    margin-left: 20px



</style>
