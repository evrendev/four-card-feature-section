<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import FooterComponent from "./components/FooterComponent.vue";
import CardComponent from "./components/CardComponent.vue";
export default {
  name: "App",
  components: {
    HeaderComponent,
    CardComponent,
    FooterComponent,
  },
};
</script>

<template>
  <main class="flex align-items-center flex-direction-column">
    <header-component />
    <div class="cards">
      <card-component
        :title="'Supervisor'"
        :description="'Monitors activity to identify project roadblocks'"
        :icon="'supervisor'"
        :theme="'bg-primary-500'"
        class="supervisor"
      />
      <card-component
        :title="'Team Builder'"
        :description="'Scans our talent network to create the optimal team for your project'"
        :icon="'team-builder'"
        :theme="'bg-primary-400'"
        class="team-builder"
      />
      <card-component
        :title="'Karma'"
        :description="'Regularly evaluates our talent to ensure quality'"
        :icon="'karma'"
        :theme="'bg-primary-600'"
        class="karma"
      />
      <card-component
        :title="'Calculator'"
        :description="'Uses data from past projects to provide better delivery estimates'"
        :icon="'calculator'"
        :theme="'bg-primary-700'"
        class="calculator"
      />
    </div>
    <footer-component />
  </main>
</template>

<style lang="scss">
@import "@/assets/styles/app.scss";
</style>
