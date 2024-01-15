<template>
    <div :key="tasks.id" v-for="task in tasks">
       <Task @delete-task="$emit('delete-task', tasks.id)" :tasks="task" />
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

