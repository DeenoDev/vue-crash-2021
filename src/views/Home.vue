<template>
    <div v-show="showAddTask" >
    <AddTask @add-task="addTask"/>
  </div>
  <Tasks @toggle-reminder="toggleReminder" @delete-task="deleteTask" :tasks="tasks" />
</template>

<script>
  import Tasks from './components/Tasks';
  import AddTask from './components/AddTask';
</script>