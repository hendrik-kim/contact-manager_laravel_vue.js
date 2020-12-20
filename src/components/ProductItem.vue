<template>
  <div class="product-item">
    <p>{{ product.name }}</p>
  </div>
</template>

<script>
export default {
  name: 'ProductItem',
  props: ['product'],
};
</script>

<style scoped></style>
