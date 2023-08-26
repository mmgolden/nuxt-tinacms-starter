<template>
  <div class="intro">
    <div class="intro__logos">
      <img src="~/assets/icon-green.svg" alt="Nuxt logo" class="intro__nuxt" />
      <p class="intro__plus">+</p>
      <img src="~/assets/tina-icon.png" alt="Tina logo" class="intro__tina" />
    </div>
    <h1 class="intro__title">Welcome to the Nuxt Tina CMS Starter!</h1>
  </div>
</template>

<script setup lang="ts"></script>

<style scoped>
.intro {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
  padding: 16px;
}

.intro__logos {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 36px;
}

.intro__nuxt {
  width: 100%;
  height: 100px;
}

.intro__plus {
  color: #ffffff;
  font-size: 48px;
  margin: 0 36px;
}

.intro__tina {
  width: 100%;
  height: 80px;
  align-self: flex-start;
}

.intro__title {
  color: #ffffff;
  font-weight: 400;
  text-align: center;
  font-size: 36px;
  margin: 0;
}

@media screen and (min-width: 767px) {
  .intro__title {
    font-size: 48px;
  }
}
</style>
