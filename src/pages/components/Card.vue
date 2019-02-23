<template>
  <q-card inline style="width: 350px" class="relative-position">
    <q-item>
      <q-item-side left >
        <img :src="card.iconImg" style="width: 50px; height: 50px" />
      </q-item-side>
      <q-item-main class="relative-position">
        <q-item-tile label class="text-weight-medium">{{card.name}}</q-item-tile>
        <q-item-tile sublabel class="text-weight-medium">{{card.header}}</q-item-tile>
      </q-item-main>
      <q-item-side right >
        <q-checkbox v-model="card.isActive" />
      </q-item-side>
    </q-item>
    <q-card-separator/>
    <q-card-main>
      <p class="text-weight-regular">{{card.description}}</p>
    </q-card-main>
  </q-card>
</template>

<script>
export default {
  props: ['card']
}
</script>

<style>
</style>
