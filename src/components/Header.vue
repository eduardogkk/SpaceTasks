<script lang="ts" setup>
  import {PhRocketLaunch} from "@phosphor-icons/vue"
</script>

<template>
  <header class="header">
    <div>
      <div class="icon"><ph-rocket-launch :size="33"/></div>
      <strong class="strongSpace">Space</strong>
      <strong class="strongTask">Task</strong>
    </div>
  </header>
</template>

<style scoped>
  .header {
    background: var(--gray-700);
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 4rem 0;
  }

  .header div {
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 1.5rem;
  }

  .strongSpace {
    color: var(--blue);
  }

  .strongTask {
    color: var(--purple);
  }

  .icon {
    color: var(--blue);
  }

</style>