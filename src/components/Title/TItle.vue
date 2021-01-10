<template>
  <div class="wrap-heading">
    <div class="heading">
      <h3 class="heading__sub--title">{{ text }}</h3>
      <h2 class="heading__title">
        {{ title }}{{ ' ' }}
        <span>{{ subTitle }}</span>
      </h2>
    </div>
  </div>
</template>
<script>
export default {
  name: 'Title',
  props: {
    text: String,
    title: String,
    subTitle: String,
  },
};
</script>
<style lang="scss">
.wrap-heading {
  padding: 10px;
}
.heading {
  margin-bottom: 55px;
  text-align: center;
  &__sub--title {
    color: #8c8c8c;
    font-size: 1.17647rem;
    font-weight: 400;
    margin-bottom: 30px;
  }
  &__title {
    font-size: 2.11765rem;
    font-weight: 700;
    margin-bottom: 0.5rem;
    margin-top: -1.3rem;
    & span {
      color: #103dbe;
    }
  }
}
</style>
