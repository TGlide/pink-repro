<div class="container">
	<h1>Welcome to SvelteKit</h1>
	<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

	<div class="u-grid u-gap-16">
		<div class="box">
			<p>Theme I'm in:</p>
		</div>
		<div class="theme-dark">
			<div class="box">
				<p>Theme I'm in:</p>
			</div>
		</div>
	</div>
</div>

<style lang="scss">
	$theme-dark: '.theme-dark';

	.box {
		--content: ' light';

		#{$theme-dark} & {
			--content: ' dark';
		}

		p::after {
			content: var(--content);
		}
	}
</style>
