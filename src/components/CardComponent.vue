<script>
import SvgIcon from "./SvgIcon.vue";
export default {
  name: "CardComponent",
  components: {
    SvgIcon,
  },
  props: {
    title: {
      type: String,
      required: true,
    },
    description: {
      type: String,
      required: true,
    },
    icon: {
      type: String,
      required: true,
    },
    theme: {
      type: String,
      required: true,
    },
  },
};
</script>

<template>
  <div class="card">
    <h1 class="fs-700 fw-semi-bold">
      {{ title }}
    </h1>
    <p class="fs-300 text-neutral-900 fw-regular opacity-50">
      {{ description }}
    </p>
    <div class="icon flex justify-content-end">
      <svg-icon :name="icon" />
    </div>
  </div>
</template>

<style lang="scss" scoped>
@import "@/assets/styles/card.scss";
</style>
