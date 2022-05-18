<template>
  <section class="comics">
    <div class="container">
      <div class="section-tag">Current Series</div>
      <div class="comics__list">
        <ProductItem
          v-for="(comic, index) in comicList"
          :key="index"
          :item="comic"
        />
      </div>
    </div>
  </section>
</template>

<script>
import ProductItem from "./ProductItem.vue";

export default {
  name: "ProductList",
  components: {
    ProductItem,
  },
  props: {
    comicList: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import "../style/common.scss";
.comics {
  background-color: $main-bg-grey;

  &__list {
    display: flex;
    flex-wrap: wrap;
  }
  .container {
    position: relative;
    padding: 2rem 0;
  }
  .section-tag {
    background-color: $brand-primary-color;
    display: inline-block;
    padding: 0.5rem;
    color: white;
    text-transform: uppercase;
    position: absolute;
    top: -1rem;
    left: 0;
  }
}
</style>
