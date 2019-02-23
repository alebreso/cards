<template>
  <div class='row gutter-xs'>
    <app-card
      v-for='card in cards'
      :key='card.id'
      :card='card'
      class="q-mt-md q-mx-sm bg-white col-auto"></app-card>
  </div>
</template>

<script>
import CardVue from './Card.vue'
export default {
  props: [ 'cards' ],
  components: {
    'appCard': CardVue
  }
}
</script>

<style>
  .bg-color {
    background-color: white;
  }

</style>
