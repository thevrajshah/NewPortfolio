<script lang="ts">
	import { blur } from 'svelte/transition';
	import { quintOut } from 'svelte/easing';
</script>

<main id="hero">
	<div class="container">
		<div class="name">
			<h5><b>vraj</b>shah</h5>
			<p>
				(works at <a href="http://www.bluelearn.in" target="_blank" rel="noopener noreferrer"
					>bluelearn</a
				>)
			</p>
		</div>
		<p
			in:blur={{ amount: 50, easing: quintOut, duration: 500 }}
			out:blur={{ amount: 50, easing: quintOut, duration: 500 }}
			class="title"
		>
			portfolio website or smth, idk
		</p>
		<div class="quote">
			<h5>just leaving my div here, can you look after it? brb!</h5>
			<h2>
				<b>
					{'<div>'}
				</b>
			</h2>
			<!-- <p>
				(works at <a href="http://www.bluelearn.in" target="_blank" rel="noopener noreferrer"
					>bluelearn</a
				>)
			</p> -->
		</div>
	</div>
</main>

<style>
	#hero {
		min-height: 100vh;
		background-image: url("data:image/svg+xml,%3C!-- svg: first layer --%3E%3Csvg viewBox='0 0 250 250' opacity='0.2' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noiseFilter'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='1000' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noiseFilter)'/%3E%3C/svg%3E"),
			radial-gradient(
				circle at top right,
				var(--gradient-4) 16%,
				var(--gradient-3) 32%,
				var(--gradient-2) 48%,
				var(--gradient-1) 64%,
				var(--gradient-0) 100%
			);
	}

	#hero .container {
		min-height: inherit;
		position: relative;
		padding-top: 1.2rem;
		padding-bottom: 1.2rem;
	}

	#hero .title {
		position: absolute;
		top: 1.2rem;
	}
	#hero .name {
		position: absolute;
		top: 1.2rem;
		right: 1rem;
		text-align: right;
	}
	#hero .quote {
		position: absolute;
		bottom: 2rem;
		right: 1rem;
		max-width: 54rem;
		text-align: right;
	}
</style>
