<script setup lang="ts">
import HappyCard from './common/HappyCard.vue';
</script>

<template>
  <section class="home">
    <HappyCard class="happiness">
      <h3 class="title">
        +8.75 %
        <i class="icon up-icon" />
      </h3>
      <p class="text">Variación Diaria de la <strong>Alegría</strong></p>
    </HappyCard>
    <HappyCard class="sad">
      <h3 class="title">
        +8.75 %
        <i class="icon up-icon" />
      </h3>
      <p class="text">Variación Diaria de la <strong>Alegría</strong></p>
    </HappyCard>
    <HappyCard class="fear">
      <h3 class="title">
        +8.75 %
        <i class="icon up-icon" />
      </h3>
      <p class="text">Variación Diaria de la <strong>Alegría</strong></p>
    </HappyCard>
    <HappyCard class="calendar">
      <h3 class="title">
        +8.75 %
        <i class="icon up-icon" />
      </h3>
      <p class="text">Variación Diaria de la <strong>Alegría</strong></p>
    </HappyCard>
    <HappyCard class="emotions">
      <h3 class="title">
        +8.75 %
        <i class="icon up-icon" />
      </h3>
      <p class="text">Variación Diaria de la <strong>Alegría</strong></p>
    </HappyCard>
    <HappyCard class="attendance">
      <h3 class="title">
        +8.75 %
        <i class="icon up-icon" />
      </h3>
      <p class="text">Variación Diaria de la <strong>Alegría</strong></p>
    </HappyCard>
  </section>
</template>

<style scoped>
  .home {
    display: grid;
    grid-template-areas: 'happiness sad fear calendar'
                         'emotions emotions emotions calendar'
                         'attendance attendance attendance calendar';
    grid-template-columns: 1fr 1fr 1fr 2fr;
    grid-template-rows: 1fr 2fr 2fr;
    gap: 16px 24px;
    width: 100%;
    height: 100%;
  }
  .happiness {
    grid-area: happiness;
  }
  .sad {
    grid-area: sad;
  }
  .fear {
    grid-area: fear;
  }
  .calendar {
    grid-area: calendar;
  }
  .emotions {
    grid-area: emotions;
  }
  .attendance {
    grid-area: attendance;
  }
</style>