<template>
  <div>
    <Header />
    <ul v-if="carts.length" class="why-choose-us__cart-list">
      <Cart v-for="cart in carts" :key="cart.id" :cart="cart" />
    </ul>
  </div>
</template>
<script>
import axios from 'axios';
import Cart from '../components/cart/Cart.vue';
import Header from '../../components/Header/Header.vue';

export default {
  name: 'HomePage',
  components: {
    Cart,
    Header,
  },
  data() {
    return {
      carts: [],
      errors: [],
    };
  },
  created() {
    axios
      .get('https://v9mjo.sse.codesandbox.io/carts')
      .then((response) => {
        this.carts = response.data;
      })
      .catch((e) => {
        this.errors.push(e);
      });
  },
};
</script>
<style lang="scss">
.why-choose-us {
  text-align: center;
  padding: 0 30px;
  &__cart-list {
    font-family: 'Be Vietnam', sans-serif;
    display: flex;
    padding-bottom: 85px;
  }

  &__img {
    margin-bottom: 22px;
  }
  &__title {
    font-size: 1.41176rem;
    font-weight: 500;
    margin-bottom: 16px;
  }
  &__desc {
    color: #5a5a5a;
  }
}
.mt-90 {
  margin-top: 90px;
}
</style>
