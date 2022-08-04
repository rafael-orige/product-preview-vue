<template>
  <ProductArea />
</template>

<script>
import { defineComponent } from 'vue';
import ProductArea from './components/Product/ProductArea.vue';

export default defineComponent({
  name: 'App',
  components: {
    ProductArea,
  },
});
</script>
