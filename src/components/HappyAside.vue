<script setup lang="ts">
import { ref } from 'vue';

const toggleAnalytics = ref(false);
</script>

<template>
  <aside class="aside">
    <nav class="aside-nav">
      <router-link class="nav-item active" to="/">
        <i class="icon home-icon" />
        Inicio
      </router-link>
      <router-link class="nav-item" to="/assistance">
        <i class="icon assistance-icon" />
        Asistencia
      </router-link>
      <router-link class="nav-item" to="/polls">
        <i class="icon polls-icon" />
        Encuestas
      </router-link>
      <button class="nav-item" @click="toggleAnalytics = !toggleAnalytics">
        <i class="icon analytics-icon" />
        Analíticas
        <i v-if="!toggleAnalytics" class="icon arrow-down-icon submenu-icon" />
        <i v-else class="icon arrow-up-icon submenu-icon" />
      </button>
      <template v-if="toggleAnalytics">
        <router-link class="nav-item subnav-item" to="/analytics/emotions">
          <i class="icon emotions-icon" />
          Emotions index
        </router-link>
        <router-link class="nav-item subnav-item" to="/analytics/emotions">
          <i class="icon wear-icon" />
          Desgaste
        </router-link>
      </template>
      <router-link class="nav-item" to="/personal">
        <i class="icon personal-icon" />
        Personal
      </router-link>
      <router-link class="nav-item" to="/departments">
        <i class="icon departments-icon" />
        Departamentos
      </router-link>
      <router-link class="nav-item" to="/settings">
        <i class="icon settings-icon" />
        Ajustes
      </router-link>
      <router-link class="logout" to="/logout">
        <i class="icon exit-icon" />
        Cerrar sesion
      </router-link>
    </nav>
  </aside>
</template>

<style scoped>
  .aside {
    width: 100%;
    height: 100%;
    padding: 110px 30px 42px;
    border-right: 1px solid var(--secondary-120);
    background: url('logo.svg') no-repeat top 36px left 33px;
  }
  .aside-nav {
    display: flex;
    flex-flow: column nowrap;
    justify-content: flex-start;
    align-items: stretch;
    gap: 10px;
    height: 100%;
  } 

  .nav-item {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    gap: 16px;
    height: 50px;
    padding-left: 16px;
    padding-right: 16px;
    border-radius: 0 10px 10px 0;
    border-left: 3px solid transparent;
    text-transform: uppercase;
    font-family: 'Open Sans';
    font-size: 14px;
    color: black;
    cursor: pointer;
    transition: background-color 0.3s, color 0.3s, border-left 0.3s;
  }
  .subnav-item {
    transform: translateX(30px);
  }
  .submenu-icon {
    margin-left: auto;
  }
  .nav-item.active,
  .nav-item:hover {
    background-color: var(--secondary-60);
    border-left: 3px solid var(--secondary-120);
    color: var(--secondary-120);
  }
  .logout {
    display: flex;
    justify-content: start;
    align-items: center;
    gap: 9px;
    margin-top: auto;
    height: 50px;
    padding-left: 26px;
    border-radius: 6px;
    font-family: 'Montserrat';
    font-size: 16px;
    color: black;
    background-color: var(--primary-60);
  }
</style>