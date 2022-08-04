<script>

import ProductImageDesktop from '../../assets/image-product-desktop.jpg';

import ButtonComponent from '../Button/ButtonComponent.vue';

export default {
  name: 'ProductArea',
  components: {
    ButtonComponent,
  },
  data() {
    return {
      image: ProductImageDesktop,
    };
  },
};

</script>

<template>
  <div class="wrapper">
    <img class="image" :src="image" alt="">
    <div class="meta">
      <h2 class="category">PERFUME</h2>
      <h1 class="title">Gabrielle Essence Eau De Parfum</h1>
      <p class="description">
        A floral, solar and voluptuous interpretation composed by Oliver Polge,
        Perfumer-Creator for the House of CHANEL.
      </p>
      <div>
        <h1 class="price"><strong>$149.99</strong></h1>
        <h2 class="discount">$169.99</h2>
      </div>
      <ButtonComponent msg="Add to Cart" />
    </div>
  </div>
</template>

<style src="./ProductArea.style.scss" lang="scss" />
