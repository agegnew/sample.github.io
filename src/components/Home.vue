<template>
  <div class="home">
    <section class="hero is-medium is-primary is-bold">
      <div class="hero-body">
        <div class="container column is-two-thirds">
          <h1 class="title">
            Welcome to my Sample vue.js project
          </h1>
          <h2 class="subtitle is-4">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus, 
            iure inventore vero debitis dignissimos rerum similique hic quia animi accusamus numquam 
            nam reprehenderit aliquid at assumenda, fugit a fugiat necessitatibus.
          </h2>
          <a class="button is-large is-primary" id="learn">Learn more</a>

        </div>

      </div>
    </section>

    <section class="section">
      <div class="container columns">
        <div class="column is-1 has-text-centered">
          <i class="fa fa-cog is-primary"></i>
        </div>
        <div class="column is-one-third-desktop">
          <p class='title'>
            <strong>we give services that you won't get anywhere else</strong>
          </p>

        </div>
        <div class="column">
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit.
            Tenetur architecto illum fuga. Porro, optio at debitis eligendi doloremque cum obcaecati 
            praesentium consequuntur repellat possimus, laboriosam enim ad consequatur libero velit! 
          </p>

        </div>
      </div>
    <div class="columns pd">
      <div class="column">
        <div class="card">
          <div class="card-content">
            <p class="title">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Animi expedita 
                            eaque atque repudiandae vel harum accusantium 
                            
            </p>
            <p class="subtitle"> -Agegnew Mersha</p>
          </div>
        </div>
      </div>
      <div class="column">
        <div class="card"> 
          <div class="card-content">
            <p class="title">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Animi expedita 
                            eaque atque repudiandae vel harum accusantium 
                            
            </p>
            <p class="subtitle"> -Agegnew Mersha</p>
          </div>
        </div>
      </div>
      <div class="column">
        <div class="card">
          <div class="card-content">
            <p class="title">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Animi expedita 
                            eaque atque repudiandae vel harum accusantium 
                           
            </p>
            <p class="subtitle"> -Agegnew Mersha</p>
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
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='sass' scoped>
@import '../mq.sass'


  
.hero
  //
  background-image: linear-gradient(to bottom, rgba(2, 30, 83, 0.808), rgba(3, 119, 134, 0.808)),url('../assets/background.jpg') !important
  background-size: cover

  .title
   
    +mobile
      font-weight: bold
    +tablet
      font-size: 2.5rem
    +desktop
      margin-left: -150px
      font-size: 4rem
      margin-top: 2rem
  

h2
  margin:1.5rem 0 2rem 0 !important

.fa-cog
  font-size: 40px
  color: rgb(50, 255, 84)
    
.pd
  background-color: rgba(4, 155, 155, 0.493)

  +tablet
    padding: 2em 0

  

</style>
