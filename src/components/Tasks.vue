<template>
    <div :key="tasks.id" v-for="task in tasks">
       <Task :tasks="task" />
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
        Task
    }
  }
</script>

