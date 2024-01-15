<template>
  <article class="bread-crumbs">
    <p class="title">Asistencia</p>
    <p class="subtitle">Asistencias de todo el personal</p>
  </article>
</template>

<style scoped>
  .bread-crumbs {
    flex-grow: 1;
    display: flex;
    flex-flow: column nowrap;
    justify-content: flex-start;
    align-items: flex-start;
  }
  .title {
    font-family: 'Montserrat';
    font-weight: 500;
    font-size: 20px;
    color: black;
  }
  .subtitle {
    font-family: 'Montserrat';
    font-weight: 500;
    font-size: 14px;
    color: var(--secondary-120);
  }
</style>