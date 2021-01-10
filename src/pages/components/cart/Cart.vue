<template>
  <div class="why-choose-us">
    <div class="why-choose-us__img">
      <img v-bind:src="cart.img" alt="#" />
    </div>
    <h3 class="why-choose-us__title">{{ cart.title }}</h3>
    <p class="why-choose-us__desc">{{ cart.desc }}</p>
  </div>
</template>
<script>
export default {
  name: 'Cart',
  props: {
    cart: {
      type: Object,
      required: true,
    },
  },
};
</script>
<style lang=""></style>
