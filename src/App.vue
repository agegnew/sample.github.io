<template>
  <div id="app">

    <nav class="navbar has-navbar-fixed-top" role="navigation" aria-label="main navigation">
      <div class="navbar-brand navbar-right">
        <a class="navbar-item" href="">
          <img style="padding: 0;margin: -1em;" src="./assets/logos.png" width="112" height="1000">
          <h1 style="padding: 0;margin: -1em;">Vue Sample</h1>
        </a>

        <a role="button" class="navbar-burger burger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample" v-on:click="toggleNav" v-bind:class="{ 'is-active' : isActive}">
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
        </a>
      </div>

      <div id="navbarBasicExample" class="navbar-menu navbar-left" v-bind:class="{ 'is-active' : isActive}">
        <div class="navbar-start">
          <router-link to="/" class="navbar-item r-item">Home</router-link>
          <router-link to="faq" class="navbar-item r-item">Features</router-link>
          
        
          <router-link to="faq" class="navbar-item r-item">More</router-link>

            
          
          
          <router-link to="faq" class="navbar-item r-item">About</router-link> 
        </div>

        <div class="navbar-end">
          <div class="navbar-item">
            <div class="control">
              <a class="button is-primary is-outlined">
                <strong>Sign up</strong>
              </a>
              <a class="button is-light is-outlined">
                Log in
              </a>
            </div>
          </div>
        </div>
      </div>
    </nav>

    <router-view/>

    

    <footer class="footer is-primary">
      <div class="container">
        <div class="columns">
          <div class="column">
            <p>And this is all the accounts that u can contact us!</p>
          </div>
          <div class="column has-text-right">
            <a class="icon" href="#"><i class="fa fa-facebook"></i></a>
            <a class="icon" href="#"><i class="fa fa-twitter"></i></a>
          </div>
        </div>
      </div>


    </footer>

  </div>
</template>

<script>
export default {
  name: 'App',
  data: function(){
    return{
      isActive: false
    }
  },
  methods:{
    toggleNav: function(){
      this.isActive=!this.isActive;
    }
  }

}
</script>

<style lang="sass">
@import '../node_modules/bulma/bulma.sass'
@import 'mq.sass'

.navbar
  background-color: #383838 !important
  border-bottom: solid 2px red
  padding: 0 1em
  padding-top: 1em
   
  a:hover
    color: black  !important
  a
    color: darkgray !important
  h1
    color: #fff
  .navbar-left
    +desktop
      margin-left: 30em !important
    +mobile
      background-color: #383838 !important
    +tablet
      background-color: #383838 !important
  .r-item
    color: #c1c1c1
    padding: 0.3rem 1.9rem
    +mobile
      color: white !important
    
    &:hover
      background-color: gray !important 
       
  .navbar-burger span
    background-color: #c1c1c1
    color: #fff

footer
  background-color: $primary !important
  color: #fff
  .icon
    color: #fff !important
    margin-left: 10px

  // .navbar-start
  //   color:#fff
  //   font-weigt: bold  !important
    


</style>
