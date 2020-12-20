<template>
  <div id="app">
    <Banner />
    <Navbar />
    <Products v-bind:products="products" />
  </div>
</template>

<script>
import Banner from './components/Banner';
import Products from './screens/Products';
import Navbar from './components/Navbar';

export default {
  name: 'App',
  components: {
    Products,
    Banner,
    Navbar,
  },
  data() {
    return {
      products: [
        {
          id: 1,
          name: 'boardwalk',
          color: 'red',
        },
        {
          id: 2,
          name: 'BROADWAY 100MM',
          color: 'red',
        },
        {
          id: 3,
          name: 'BROADWAY PLANKS 100MM',
          color: 'red',
        },
      ],
    };
  },
};
</script>

<style></style>
