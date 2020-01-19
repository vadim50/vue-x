<template>
  <div class="container pt-5">
    <h1>{{ msg }}</h1>
    <app-counter></app-counter>
    <app-second-counter></app-second-counter>
    <hr>
    <app-actions></app-actions>
  </div>
</template>

<script>

import Counter from './Counter.vue'
import Actions from './Actions.vue'
import SecondCounter from './SecondCounter.vue'


export default {
 
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  components: {
    appCounter: Counter,
    appActions: Actions,
    appSecondCounter: SecondCounter
  }
}
</script>

<style>

</style>
