<template>
    <div :key="tasks.id" v-for="task in tasks">
       <Task @toggle-reminder="$emit('toggle-reminder', task.id)" @delete-task="$emit('delete-task', tasks.id)" :tasks="task" />
    </div>

</template>

<script>
import Task from './Task'

  export default {
    name: 'Tasks',
    props: {
        tasks: Array
    },
    components: {
        Task,
    },
    emits: ['delete-task'],
    
  }
</script>

