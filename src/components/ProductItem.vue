<template>
  <div class="product-item">
    <img src="" alt="" />
    <p>{{ product.name }}</p>
    <div class="product-color-container">
      <p>Select a colour</p>
      <img src="" alt="" />
    </div>
    <button class="product-item-button">+ add to proejct</button>
  </div>
</template>

<script>
export default {
  name: 'ProductItem',
  props: ['product'],
};
</script>

<style scoped></style>
