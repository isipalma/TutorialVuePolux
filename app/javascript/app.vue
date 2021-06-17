<template>
  <div class="container text-center mt-5">
    <div class="row">
      <div class="col-md-12">
 
        <div id="app">
          <h1>{{ titulo }}</h1>
          <button class="u-link-white" @click="counter_down">
            {{ counter }}
          </button>
          <Message/>
 
          <!-- Componente Postres -->
          <Postres/>
          <card-swipe>
            <card-swipe-item>
              <div style="background-image: linear-gradient(to right, #fe686c 0%, #fe3c71 100%); width: 250px; height: 60px;">1</div>
            </card-swipe-item>
            <card-swipe-item>
              <div style="background-image: linear-gradient(to right, #ffaa00 0%, #ff8800 100%); width: 250px; height: 60px;">2</div>
            </card-swipe-item>
            <card-swipe-item>
              <div style="background-image: linear-gradient(to right, #add0f8 0%, #5ca2f8 100%); width: 250px; height: 60px;">3</div>
            </card-swipe-item>
          </card-swipe>
 
        </div>
      </div>
    </div>
    
  </div>
</template>

<script>
 
  // Importo el componente 'Postres' 
  import Postres from './Postres'
  import Message from './Message'

  import { CardSwipe, CardSwipeItem } from '@eshengsky/vue-card-swipe';
 
  export default {
 
    // Defino el componente 'Postres' 
    components: {
      Postres,
      Message,
      CardSwipe,
      CardSwipeItem
    },
 
    data: function () {
      return {
        titulo: "Lista de Postres",
        counter: 200
      }
    },

    methods: {
      counter_down: function () {
        this.counter -= 1;
      }
    }
 
  }
</script>


<style scoped>
  p {
    font-size: 2em;
    text-align: center;
  }
</style>

