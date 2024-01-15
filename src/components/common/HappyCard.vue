<template>
  <article class="card">
    <slot />
  </article>
</template>

<style scoped>
.card {
  padding: 14px;
  border: 1px solid var(--secondary-60);
  border-radius: 10px;
}
</style>