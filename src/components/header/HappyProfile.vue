<template>
  <article class="profile">
    <figure class="avatar">
      <img class="avatar-img" src="@/assets/img/avatar.png" alt="Avatar">
      <figcaption class="profile-info">
        <p class="position">HR Manager</p>
        <p class="name">Mari Carmen García</p>
      </figcaption>
    </figure>
  </article>
</template>

<style scoped>
  .profile {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100%;
    padding: 5px 16px 5px 5px;
    border-radius: 10px;
    border: 1px solid var(--secondary-60);
  }
  .avatar {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    gap: 6px;
  }
  .avatar-img {
    border-radius: 8px;
  }
  .profile-info {
    display: flex;
    flex-flow: column nowrap;
    justify-content: center;
  }
  .position {
    font-family: 'Montserrat';
    font-weight: 500;
    font-size: 12px;
    color: var(--secondary-120);
  }
  .name {
    font-family: 'Montserrat';
    font-weight: 500;
    font-size: 16px;
    color: black;
  }
</style>