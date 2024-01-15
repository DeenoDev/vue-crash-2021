<template>
    <div :class="[tasks.reminder ? 'reminder' : '', 'task']">
        <h3>{{ tasks.text }}
        <i class="fas fa-times"></i>
        </h3>
        <p>{{ tasks.day }}</p>
    </div>
</template>

<script>
export default {
    name: 'Task',
    props: {
        tasks: Object,
    },
}

</script>

<style scope>
.fas {
  color: red;
}

.task {
  background: #f4f4f4;
  margin: 5px;
  padding: 10px 20px;
  cursor: pointer;
}

.task.reminder {
  border-left: 5px solid green;
}

.task h3 {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
</style>