<template>
  <div class="flex flex-col min-h-screen font-Roboto bg-weather-primary">
    <site-navigation />
    <router-view />
  </div>
</template>

<script>
import { RouterView } from "vue-router";
import SiteNavigation from "./components/SiteNavigation.vue";

export default {
  components: {
    SiteNavigation,
  },
  setup() {
    return {
      router: RouterView.router,
    };
  },
};
</script>

<style lang="scss" scoped></style>
