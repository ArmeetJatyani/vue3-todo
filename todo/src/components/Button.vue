<template>
	<button @click="onClick()" :style="variables">{{ text }}</button>
</template>

<script>
	export default {
		name: "Button",
		props: {
			text: {
				type: String,
				default: "Default Value",
			},
			bgColor: {
				type: String,
				default: "#ff85ff",
			},
			textColor: {
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
					"--bg-color": this.bgColor,
					"--text-color": this.textColor,
				};
			},
		},
		methods: {
			onClick() {
				console.log("Clicked");
				return;
			}
		},
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
		font-family: Roboto Mono, monospace;
		font-size: 16px;
		font-weight: bold;
		border-radius: 10px;

		margin-right: 100px;

		transition: all 0.1s ease-in-out;
	}

	button:hover {
		filter: brightness(90%);
	}
</style>
