<template>
  <div class="container">
    <AppHeader/>
    <SocialBar/>
    <nuxt/>
  </div>
</template>

<script>
import AppHeader from "../components/AppHeader";
import SocialBar from "../components/SocialBar";
export default {
  components: {
    AppHeader,
    SocialBar
  }
};
</script>

<style>

</style>