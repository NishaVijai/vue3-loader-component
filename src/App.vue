<template>
  <main>
    <!-- <UserCard />
    <UserCardSkeleton /> -->
    <Suspence>
      <UserCard />
      <template #fallback>
        <UserCardSkeleton />
      </template>
    </Suspence>
  </main>
</template>

<script>
import UserCard from "./components/UserCard.vue";
import UserCardSkeleton from "./components/UserCardSkeleton.vue";

export default {
  name: "App",
  components: {
    UserCard,
    UserCardSkeleton,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Mouse+Memoirs&display=swap");

*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Mouse Memoirs", sans-serif;
}

main {
  max-width: 620px;
  margin: 0 auto;
  padding-top: 32px;
  display: flex;
  flex-direction: column;
  gap: 16px;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
