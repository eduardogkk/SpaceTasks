<script lang="ts" setup>
  import {PhRocketLaunch} from "@phosphor-icons/vue"
</script>

<template>
  <header class="header">
    <strong>
      <ph-rocket-launch :size="33"/>
      SpaceTasks
    </strong>
  </header>
</template>

<style>
  .header {
    background: var(--gray-700);
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 4rem 0;
  }

  .header strong {
    display: flex;
    color: var(--blue);
    font-size: 1.5rem;
  }

</style>