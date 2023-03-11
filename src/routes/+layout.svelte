<slot />

<style>
	@import url('https://fonts.googleapis.com/css2?family=Golos+Text:ital,wght@0,400;0,700;1,400&display=swap');

	:global(:root) {
		--gradient-0: #291e3c;
		--gradient-1: #22214d;
		--gradient-2: #2d0d8d;
		--gradient-3: #500d7e;
		--gradient-4: #5403a5;
	}

	:global(*) {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}

	:global(html) {
		font-size: 100%;
	}

	:global(body) {
		font-weight: 400;
		font-family: 'Golos Text', serif;
		line-height: 1.75;
		color: hsl(281, 24%, 80%);
		background: var(--gradient-1);
		box-sizing: border-box;
	}

	:global(.container) {
		margin: 0 auto;
		max-width: 80rem;
		padding: 0 1rem;
	}

	:global(p) {
		margin-bottom: 1rem;
	}

	:global(a) {
		text-decoration: none;
		color: hsl(281, 100%, 87%);
	}
	:global(a:hover) {
		text-decoration: underline;
		color: hsl(281, 100%, 80%);
	}

	:global(h1, h2, h3, h4, h5) {
		/* margin: 3rem 0 1.38rem; */
		/* font-family: 'Poppins', sans-serif; */
		font-weight: 400;
		line-height: 1.3;
	}

	:global(h1) {
		margin-top: 0;
		font-size: 7.594rem;
	}

	:global(h2) {
		font-size: 5.063rem;
	}

	:global(h3) {
		font-size: 3.375rem;
	}

	:global(h4) {
		font-size: 2.25rem;
	}

	:global(h5) {
		font-size: 1.5rem;
	}

	:global(small) {
		font-size: 0.667rem;
	}

	@media only screen and (max-width: 600px) {
		:global(html) {
			font-size: 80%;
		}
	}
</style>
