<template>
	<div class="container">
		<Header />
	</div>
</template>

<script>
	import Header from "@/components/Header.vue";

	export default {
		name: "App",
		components: {
			Header,
		},
	};
</script>

<style>
	@tailwind base;
	@tailwind components;
	@tailwind utilities;

	#app {
		--monospaced-font: Roboto Mono, monospace;
		--main-font: Roboto, Arial, Helvetica, sans-serif;
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
	}
</style>
