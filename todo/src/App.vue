<template>
	<Header />
	<Tasks :tasks="tasks" />
</template>

<script>
	import Header from "@/components/Header.vue";
	import Tasks from "@/components/Tasks.vue";

	export default {
		name: "App",
		components: {
			Header,
			Tasks,
		},
		data() {
			return {
				tasks: [],
			};
		},
		created() {
			this.tasks = [
				{
					id: 1,
					text: "Do the dishes",
					day: "3-16-2020",
				},
				{
					id: 2,
					text: "Brush teeth",
					day: "3-16-2020",
				},
				{
					id: 3,
					text: "Mop house",
					day: "3-16-2020",
				},
				{
					id: 4,
					text: "Do HW",
					day: "3-16-2020",
				},
				{
					id: 4,
					text: "Laundry",
					day: "3-16-2020",
				},
			];
		},
	};
</script>

<style>
	:root {
		/* @import url("./css/variables.css"); */

		/** COLORS */
		--bg-color: #091f2c;
		--primary-color: #ff85ff;
		--secondary-color: #ff6fff;

		/** FONTS */
		--monospaced-font: Roboto Mono, monospace;
		--main-font: Roboto, Arial, Helvetica, sans-serif;
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;

		background: var(--bg-color);
		color: var(--primary-color);

		margin: 0px;
		padding: 0px;
	}

	#app {
	}
</style>
