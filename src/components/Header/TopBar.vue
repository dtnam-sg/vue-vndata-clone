<template>
  <div class="wraper">
    <b-container>
      <b-row>
        <b-col md="6">
          <ul class="top-bar top-bar__left">
            <li><i class="fas fa-phone"></i>0971-05-4444</li>
            <li><i class="far fa-envelope"></i>info@vndata.vn</li>
          </ul>
        </b-col>
        <b-col md="6">
          <ul class="top-bar top-bar__right">
            <li><i class="fas fa-phone"></i>Đăng nhập</li>
            <li><i class="far fa-envelope"></i>Đăng ký</li>
          </ul>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>
<script>
export default {
  name: 'TopBar',
};
</script>
<style lang="scss">
.wraper {
  background-color: rgb(21, 9, 94);
  color: #fff;
  font-size: 0.88235rem;
  padding: 15px 0;
}
.top-bar {
  display: flex;
  margin-left: -8px;
  &__left {
    & li:first-child {
      margin-right: 58px;
    }
  }
  &__right {
    justify-content: flex-end;
    margin-left: -12px;
    & li:first-child {
      margin-right: 35px;
    }
  }
}
li i {
  padding-right: 8px;
}
</style>
