<template>
	<button :style="variables">{{ text }}</button>
</template>

<script>
	export default {
		name: "Button",
		props: {
			text: {
				type: String,
				default: "Default Value",
			},
			"bg-color": {
				type: String,
				default: "#ff85ff",
			},
			"text-color": {
				type: String,
				default: "#091f2c",
			},
			w: {
				type: String,
				default: "100px",
			},
			h: {
				type: String,
				default: "50px",
			},
		},
		computed: {
			variables() {
				return {
					"--w": this.w,
					"--h": this.h,
					"--bg-color": this["bg-color"],
					"--text-color": this["text-color"],
				};
			},
		},
		methods: {},
		components: {},
	};
</script>

<style scoped>
	button {
		background-color: var(--bg-color);
		color: var(--text-color);
		width: var(--w);
		height: var(--h);

		outline: 0px;
		border: 0px;
		cursor: pointer;

	}

	button:hover {
	}
</style>
