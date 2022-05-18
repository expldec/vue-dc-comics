<template>
  <div class="comics__item">
    <img :src="item.thumb" alt="item.series" />
    <h3>{{ item.series }}</h3>
  </div>
</template>

<script>
export default {
  name: "ProductItem",
  props: {
    item: Object,
  },
};
</script>

<style lang="scss" scoped>
.comics__item {
  width: calc(100% / 6);
  padding: 0.5rem;
  h3 {
    color: white;
    font-size: 1rem;
    text-transform: uppercase;
    font-weight: 300;
  }
}
</style>
