<script setup>
import HomePage from "./components/HomePage.vue";
import HomeRight from "./components/HomeRight.vue";
</script>

<template>
  <header>
    <img
      alt="Vue logo"
      class="logo"
      src="./assets/logo.png"
      width="125"
      height="125"
    />

    <div class="wrapper">
      <HomePage msg="taxable" />
      
    </div>
  </header>

  <main>
   <div>
    <HomeRight />
   </div>
 </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
