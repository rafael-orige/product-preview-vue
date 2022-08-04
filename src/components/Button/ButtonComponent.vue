<script>
import CartIcon from '../../assets/icon-cart.svg';

export default {
  name: 'ButtonComponent',
  props: {
    msg: {
      type: String,
      required: true,
    },
  },
  data() {
    return {
      image: CartIcon,
    };
  },
};
</script>

<template>
  <button>
    <img :src="image" />
    {{msg ? msg : 'Fill {msg}'}}
  </button>
</template>

<style src="./ButtonComponent.style.scss" lang="scss" scoped />
