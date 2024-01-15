<template>
  <article class="search">
    <label for="search" class="sr-only">Busqueda</label>
    <i class="icon search-icon" />
    <input class="input" type="text" id="search" name="search" placeholder="Búsqueda">
  </article>
</template>

<style scoped>
  .search {
    display: flex;
    flex-flow: row nowrap;
    justify-content: flex-start;
    align-items: center;
    height: 100%;
    padding: 13px 16px;
    border: 1px solid var(--secondary-60);
    border-radius: 10px;
  }
  .icon {
    color: var(--secondary-120);
  }
  .input {
    width: 205px;
    height: 100%;
    padding-left: 10px;
    border: none;
    background-color: transparent;
    font-family: 'Montserrat';
    font-weight: 400;
    font-size: 16px;
    color: black;
  }
</style>
