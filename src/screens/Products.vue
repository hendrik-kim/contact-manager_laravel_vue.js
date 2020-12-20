<template>
  <div>
    <div v-bind:key="product.id" v-for="product in products">
      <ProductItem v-bind:product="product"></ProductItem>
    </div>
  </div>
</template>

<script>
import ProductItem from '../components/ProductItem';
export default {
  name: 'Products',
  components: {
    ProductItem,
  },
  props: ['products'],
};
</script>

<style scoped></style>
