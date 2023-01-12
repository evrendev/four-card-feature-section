<script>
import HeaderComponent from "./components/HeaderComponent.vue";
export default {
  name: "App",
  components: {
    HeaderComponent,
  },
};
</script>

<template>
  <main>
    <header-component />
  </main>
</template>

<style lang="scss">
@import "@/assets/styles/app.scss";
</style>
