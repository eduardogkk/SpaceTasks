<template>
  <article class="taskList">
    <header class="header">
      <div>
        <strong class="strongCreated">Tarefas Criadas<span>2</span></strong>
        <strong class="strongDone">Concluídas<span>1</span></strong>
      </div>
    </header>

    <div class="tasks">
      <div class="task1">
        <h3>Task</h3>
        <p>Tasks para fazer</p>
      </div>
      <div class="task2">
        <h3>Task</h3>
        <p>Tasks para fazer</p>
      </div>
      <div class="task3">
        <h3>Task</h3>
        <p>Tasks para fazer</p>
      </div>
      <div class="task4">
        <h3>Task</h3>
        <p>Tasks para fazer</p>
      </div>
    </div>
  </article>
</template>

<style scoped>
  .taskList {
    margin-top: 3rem;
    padding: 0;
    width: auto;
    height: 50rem;
  }

  .header div{
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .strongCreated {
    color: var(--blue)
  }

  .strongDone {
    color: var(--purple);
  }
  
  .header div strong span {
    color: var(--gray-200);
  }

  .header div strong span::before {
    content: "\2022";
    padding: 0 0.25rem;
  }

  .tasks {
    padding: 1.5rem 0;
  }

  .tasks div {
    padding: 0.25rem 0;  
  }

</style>