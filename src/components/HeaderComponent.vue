<template>
  <header class="flex align-items-center flex-direction-column">
    <h2 class="fw-extra-light fs-900 text-neutral-900">Reliable, efficient delivery</h2>
    <h1 class="fw-semi-bold fs-900 text-neutral-900">Powered by Technology</h1>
    <p class="fs-400 fw-regular text-neutral-900 text-center">
      Our Artificial Intelligence powered tools use millions of project data points to ensure that
      your project is successful
    </p>
  </header>
</template>

<script>
export default {
  name: "HeaderComponent",
  setup() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
header {
  max-width: 540px;

  h2 {
    letter-spacing: 0.25px;
  }

  p {
    margin-top: var(--size-400);
    line-height: var(--size-600);
    opacity: 0.5;
  }
}
</style>
