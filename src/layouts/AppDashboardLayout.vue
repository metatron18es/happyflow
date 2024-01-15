<script lang="ts" setup>
import HappyAside from '../components/HappyAside.vue';
import HappyHeader from '../components/HappyHeader.vue';
</script>

<template>
  <div class="dashboard-layout">
    <HappyAside class="dashboard-aside" />
    <HappyHeader class="dashboard-header"/>
    <main class="main">
    <slot />
  </main>
  </div>

</template>

<style scoped>
  .dashboard-layout {
    display: grid;
    grid-template-areas: 'aside header'
                         'aside main';

    grid-template-columns: 280px 1fr;
    grid-template-rows: 90px 1fr;
    width: 100%;
    height: 100%;
    overflow: hidden;
  }

  .dashboard-aside {
    grid-area: aside;
  }
  .dashboard-header {
    grid-area: header;
  }
  .main {
    grid-area: main;
    padding: 20px 32px;
    overflow-y: auto;
  }
</style>
