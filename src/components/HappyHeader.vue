<script setup lang="ts">
import HappyBreadCrumbs from './header/HappyBreadCrumbs.vue';
import HappyNotifications from './header/HappyNotifications.vue';
import HappyProfile from './header/HappyProfile.vue';
import HappySearch from './header/HappySearch.vue';
</script>


<template>
  <header class="header">
    <HappyBreadCrumbs />
    <HappySearch />
    <HappyNotifications />
    <HappyProfile />
  </header>
</template>

<style scoped>
  .header {
    display: flex;
    flex-flow: row nowrap;
    justify-content: flex-start;
    align-items: center;
    gap: 26px;
    width: 100%;
    height: 100%;
    padding: 20px 32px 20px 50px;
  }
</style>