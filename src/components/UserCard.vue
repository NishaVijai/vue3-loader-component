<script setup>
</script>

<template>
  <section class="user-card">
    <section class="card-avatar">
      <img src="../assets/profile.jpeg" alt="user profile picture" />
    </section>
    <section class="card-info">
      <p class="name">User Name</p>
      <p class="summary">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Tenetur
        doloremque labore illum accusamus, quo voluptates unde nihil quia!
        Nostrum ea accusamus explicabo beatae vero inventore.
      </p>
    </section>
  </section>
</template>

<style>
.user-card {
  display: flex;
  gap: 16px;
  padding: 30px;
  background-color: #f1f1f1;
  box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);
}

.card-avatar img {
  width: 100px;
  height: auto;
  border-radius: 50%;
  box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);
}

.card-info {
  display: flex;
  flex: 1;
  flex-direction: column;
  gap: 16px;
}

.name {
  font-size: 32px;
}

.summary {
  font-size: 20px;
}
</style>