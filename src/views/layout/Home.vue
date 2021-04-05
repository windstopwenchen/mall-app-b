<template>
  <div class="home">
    <left-menu />
    <div :class="{ 'main-app': true, 'menu-unfold': $store.state.collapsed }">
      <slider-nav />
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
import LeftMenu from './components/Menu.vue';
import SliderNav from './components/SliderNav.vue';

export default {
  data() {
    return {

    };
  },
  components: {
    LeftMenu,
    SliderNav,
  },
  methods: {},
};
</script>

<style lang="less">
@import url("~@/assets/css/home.less");
</style>
