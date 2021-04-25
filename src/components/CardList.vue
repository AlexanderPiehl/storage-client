<template>
  <div class="d-flex flex-wrap">
    <CardListItem v-for="(item, index) in items" :key="index" :item="item" />
  </div>
</template>

<script>
import CardListItem from "@/components/CardListItem";

export default {
  name: "CardList",
  components: {
    CardListItem,
  },
  props: {
    items: Array,
  },
};
</script>

<style lang="sass" scoped>
</style>