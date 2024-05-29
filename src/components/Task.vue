<script lang="ts" setup>
  import {PhTrash, PhCircle, PhCheckCircle} from "@phosphor-icons/vue"
</script>

<template>
  <div class="task">
    <button class="btnCheck" title="Check">
      <ph-circle :size="24" class="iconCircle"/>
      <ph-check-circle :size="24" class="iconCheck"/>
    </button>
    <div class="taskContent">
      <p>Conteudo da task</p>
    </div>
    <button class="btnTrash" title="Deletar task">
      <ph-trash :size="25" />
    </button>
  </div>
</template>

<style scoped>
  .task {
    background: var(--gray-500);
    margin-top: 1rem;
    border-radius: 8px;
    height: 4rem;
    display: flex;
    align-items: center;
    justify-content: space-between;
    overflow: auto;
  }

  .btnCheck {
    border: 0;
    background: transparent;
    padding: 0 0 0 1rem;
  }

  .iconCircle {
    color: var(--blue);
    transition: 0.4s;
  }

  .iconCircle:hover {
    color: var(--blue-dark);
  }

  .iconCheck {
    color: var(--purple);
    transition: 0.4s;
  }

  .iconCheck:hover {
    color: var(--purple-dark);
  }

  .taskContent {
    color: var(--gray-100);
  }

  .btnTrash {
    background: transparent;
    border: 0;
    padding: 0 1rem 0 0;
    cursor: pointer;
    color: var(--gray-300);

    transition: 0.4s;
  }

  .btnTrash:hover {
    color: var(--danger);
  }

</style>