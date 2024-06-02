<template>
  <section class="banner">
    <div class="banner__info">
      <h1 class="banner__info_header">{{ bunnerHeader }}</h1>
      <div class="banner__info_breadcrump">
        {{ bcrump }}
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "BaseBanner",
  props: {
    bunnerHeader: String,
    bcrump: String,
    image: String,
  },

  data() {
    return {};
  },

  computed: {},
};
</script>

<style lang="scss">
@import "../style/variables.scss";

.banner {
  // background-image: v-bind("image");
  background-image: v-bind("image");
  min-height: 356px;
  @include flexCenter;
  align-items: flex-end;
  &__info {
    text-align: center;
    background-color: #fff;
    padding: 41px;
    border-radius: 37px 37px 0px 0px;
    &_header {
      @include h2Style;
      text-align: left;
    }
    &_breadcrump {
      font-size: 22px;
      font-weight: 400;
      line-height: 33px;
    }
  }
}
</style>
