<template>
	<div v-for="task in tasks" :key="task.id" class="card">
		<h3>{{ task.text }}</h3>
	</div>
</template>

<script>
	export default {
		name: "Tasks",
		props: {
			tasks: {
				type: Array,
			},
		},
	};
</script>

<style>
	.card {
        margin-left: 100px;
        margin-right: 100px;
        margin-top: 80px;
    }

    .card h3 {
        font-weight: bold;
        cursor: pointer;
    }


</style>
