<template>
    <div class="task">
        <h3>{{ task.text }}</h3>
        
    </div>
</template>

<script>
export default {
    name: 'Task',
    props: {
        task: ObjectS
    }
}

</script>