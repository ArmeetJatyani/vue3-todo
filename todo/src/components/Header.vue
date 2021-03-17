<template>
	<div class="nav">
		<h1>TAQ</h1>
		<Button text="Add" w="100px" h="50px"/>
	</div>
</template>

<script>
	import Button from "@/components/Button.vue";
	export default {
	    name: "Header",
	    props: {},
	    methods: {},
	    components: {Button},
	};
</script>

<style scoped>
	.nav {
		margin: none;
		padding: none;
		display: flex;
		align-items: center;
		justify-content: space-between;
	}

	h1 {
		margin-left: 100px;
		letter-spacing: 5px;
	}
</style>
