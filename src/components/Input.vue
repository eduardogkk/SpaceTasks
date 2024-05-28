<script lang="ts" setup>
import {PhPlusCircle} from "@phosphor-icons/vue";
</script>

<template>
  <form class="CreateTaskForm">
    <textarea
      name="task"
      placeholder="Crie uma nova task!"
      ></textarea>

    <button class="buttonCreate" type="submit">
      Criar
      <ph-plus-circle :size="23" />
    </button>
  </form>
</template>

<style>
  .CreateTaskForm {
    display: flex;
    justify-content: center;
    gap: 0.85rem;
    margin-top: -1.45rem;
  }

  .CreateTaskForm textarea {
    border: 0;
    resize: none;
    height: 3.1rem;
    width: 26rem;
    padding: 0.85rem;
    background: var(--gray-500);
    border-radius: 8px;
    line-height: 1.4;
    color: var(--gray-100);

    transition: 1s;
  }

  .CreateTaskForm textarea:focus {
    background: var(--gray-400);
  }

  .CreateTaskForm textarea:hover {
    background: var(--gray-400);
  }

  .CreateTaskForm button {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 7px;
    border: 0;
    width: 6.5rem;
    border-radius: 8px;
    background: var(--blue-dark);
    color: var(--gray-100);
    font-weight: bold;
    cursor: pointer;

    transition: 1s;
}

  .CreateTaskForm button:hover {
    background: var(--blue);
  }
</style>