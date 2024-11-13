<script lang="ts">
	import '../app.css';
	let { children } = $props();
</script>

<style>

	:global(html, body) {
		@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

		font-family: "Poppins", sans-serif;
		background-color: #152a55;
		color: white;
		margin: 0;
		height: 100%;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;

		.brand {
			display: flex;
			justify-content: center;
			align-items: center;
			margin-bottom: 0.5rem;

			.circle {
				width: 4rem;
				height: 4rem;
				border-radius: 100%;
				border-top: transparent 0.75rem solid;
				border-bottom: white 0.75rem solid;
				border-left: white 0.75rem solid;
				border-right: white 0.75rem solid;
				background-color: transparent;
				margin-right: 0.5rem;
				position: relative;
			}

			.circle::before {
				content: "";
				width: 1.5rem;
				height: 1.5rem;
				border-radius: 100%;
				background-color: white;
				position: absolute;
				top: 50%;
				left: 50%;
				transform: translate(-50%, -50%);
			}

			.title {
				width: 13rem;
				font-size: 1.5rem;
				line-height: 2rem;
			}
		}
	}

</style>

<div class="brand">
	<div class="circle"></div>
	<h1 class="title">Expo Empresarial Camcaroní 2024</h1>
</div>

{@render children()}
