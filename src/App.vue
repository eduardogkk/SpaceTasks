<script setup lang="ts">
import Header from "./components/Header.vue"
import Input from "./components/Input.vue"
import TaskList from "./components/TaskList.vue";
</script>

<template>
  <div>
    <Header />
      <div class="wrapper">
        <main>
        <Input />
        <TaskList />
      </main>
      </div>
  </div>
</template>

<style>
  :root {
  --gray-100: #F2F2F2;
  --gray-200: #D9D9D9;
  --gray-300: #808080;
  --gray-400: #333333;
  --gray-500: #262626;
  --gray-600: #1A1A1A;
  --gray-700: #0D0D0D;

  --blue-dark: #1E6F9F;
  --blue: #4EA8DE;
  --purple-dark: #5E60CE;
  --purple: #8284FA;

  --danger: #E25858;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background: var(--gray-600);
  color: var(--gray-100);
  -webkit-font-smoothing: antialiased;
}

body,
textarea,
button,
input, p {
  font-family: "inter", sans-serif;
  font-weight: 400;
  font-size: 1rem;
}

  .wrapper {
  max-width: 50rem;
  margin: auto;

  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
</style>
