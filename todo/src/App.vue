<template>
	<Header />
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
