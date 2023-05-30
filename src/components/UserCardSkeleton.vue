<template>
  <section class="user-card">
    <section class="card-avatar">
      <AnimatedPlaceholder height="100px" width="100px" borderRadius="50%" />
    </section>
    <section class="card-info">
      <AnimatedPlaceholder height="36px" width="200px" />
      <section class="summary-placeholder">
        <AnimatedPlaceholder height="16px" />
        <AnimatedPlaceholder height="16px" />
        <AnimatedPlaceholder height="16px" />
      </section>
    </section>
  </section>
</template>

<script>
import AnimatedPlaceholder from "./AnimatedPlaceholder.vue";

export default {
  name: "UserCardSkeleton",
  components: {
    AnimatedPlaceholder,
  },
};
</script>

<style scoped>
.summary-placeholder {
  display: flex;
  flex-direction: column;
  gap: 8px;
  width: 100%;
}
</style>
