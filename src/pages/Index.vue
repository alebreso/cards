<template>
  <div class='featured q-mb-none q-mx-auto'>
    <q-page>
      <h3 class='q-my-none'>Featured</h3>
      <app-card-list :cards='cards' class="flex q-my-lg"></app-card-list>
    </q-page>
  </div>
</template>

<style>
  .featured {
    width: 90%;
    background-color: #ffffffdb;
  }
</style>

<script>
import cardListVue from './components/cardList.vue'
export default {
  name: 'PageIndex',
  data: function () {
    return {
      cards: [
        { id: 1, iconImg: '../../statics/images/Kira-thumbnail.png', name: 'Kira', header: "It's How You Know What's In Your Contracts", description: 'Kira is a powerful machine learning software that identifies, extract and analizes text in your contracts and other documents.', isActive: false },
        { id: 2, iconImg: '../statics/images/Doxly-thumbnail.png', name: 'Doxly', header: 'Secure Portal for End to End Transaction', description: 'Manage the entire legal transaction process from diligence to closing.', isActive: false },
        { id: 3, iconImg: '../statics/images/Clause-thumbnail.png', name: 'Kira', header: 'Connected Contracting', description: 'Clause builds the technology infrastructure for connected contracts to increase the value and improve the managememnt of your nusiness agreements.', isActive: false }
      ]
    }
  },
  components: {
    'appCardList': cardListVue
  }
}
</script>
