<template>
  <v-card class="mx-auto">
    <v-img :src="item.photoUrl" height="200px"></v-img>

    <v-card-title> {{ item.title }} </v-card-title>

    <v-card-subtitle> {{ item.subTitle }} </v-card-subtitle>

    <v-card-text>
      {{ item.description }}
    </v-card-text>

    <v-card-actions>
      <v-btn text> Reservieren </v-btn>
    </v-card-actions>
  </v-card>
</template>

<script>
export default {
  name: "CardListItem",
  props: {
    item: Object,
  },
};
</script>

<style lang="sass" scoped>
.mx-auto
    width: 300px
</style>