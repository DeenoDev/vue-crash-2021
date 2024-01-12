<template>
    <div class="task">
        <h3>{{ tasks.text }}</h3>
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