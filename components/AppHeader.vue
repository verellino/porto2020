<template>
  <header class="header">
    <nuxt-link to="/" class="logo">
      <img src="../assets/logo.svg" alt="Mekel Verellino's Logo">
    </nuxt-link>

    <ul>
      <li>
        <nuxt-link to="/works">WORKS</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/about">ABOUT</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/contact">CONTACT</nuxt-link>
      </li>
    </ul>
  </header>
</template>

<script>
export default {
  name: "AppHeader"
};
</script>

<style>
.header {
  position: fixed;
  display: flex;
  width: calc(100vw - 160px);
  margin-top: 40px;
  justify-content: space-between;
  align-items: center;
  z-index: 100;
  mix-blend-mode: difference;
}
.header ul {
  display: flex;
}
.header li {
  display: inline-block;
  padding: 0 1rem;
  font-family: Rakkas;
}
.logo {
  height: 40px;
}

@media only screen and (min-device-width: 768px) and (max-device-width: 1280px) and (-webkit-min-device-pixel-ratio: 2) {
  .header {
    width: calc(100vw - 80px);
  }
}
@media only screen and (min-device-width: 481px) and (max-device-width: 767px) and (-webkit-min-device-pixel-ratio: 2) {
  .header {
    width: calc(100vw - 32px);
    padding-top: 16px;
  }
  .logo {
    height: 32px;
  }
}
@media only screen and (min-device-width: 300px) and (max-device-width: 480px) and (-webkit-min-device-pixel-ratio: 2) {
  .header {
    width: calc(100vw - 16px);
    padding-top: 8px;
  }
  .logo {
    height: auto;
  }
}
</style>