<script>
	import { createEventDispatcher } from 'svelte';

	const dispatcher = createEventDispatcher();

	function handleSwitch(event) {
		dispatcher('handleSwitch', { isMonthly: event.target.value });
	}
</script>

<header class="header">
	<div class="header-wrapper">
		<h1 class="heading">Our Pricing</h1>
		<div class="toggle-button-group">
			<p class="annually">Annually</p>
			<input
				on:change={handleSwitch}
				id="themeToggler"
				type="range"
				name="theme-toggle"
				min="0"
				max="1"
				value="0"
			/>
			<p class="monthly">Monthly</p>
		</div>
	</div>
</header>

<style>
	.header {
		padding-top: 4rem;
		padding-right: 4.25rem;
		padding-left: 4.25rem;
	}
	.header-wrapper {
	}

	.heading {
		font-size: 2rem;
		text-align: center;
		font-weight: 700;
		color: var(--grayish-blue);
	}
	.toggle-button-group {
		display: flex;
		align-items: center;
		justify-content: center;
		gap: 24px;
		margin-top: 40px;
	}
	.annually,
	.monthly {
		font-size: 0.9375rem;
		opacity: 0.5;
		font-weight: 700;
		color: var(--grayish-blue);
		line-height: 1.86;
	}

	input[type='range'] {
		-webkit-appearance: none;
		appearance: none;
		background: var(--primary);
		height: 32px;
		width: 56px;
		border-radius: 16px;
		cursor: pointer;
	}

	input[type='range']::-webkit-slider-thumb {
		/* for webkit or blink powered browser */
		-webkit-appearance: none;
		background: white;
		height: 24px;
		width: 24px;
		border-radius: 13px;
	}
	input[type='range']::-ms-tooltip {
		display: none;
	}
	input[type='range']::-moz-range-track {
		height: 0;
	}
	input[type='range']::-moz-range-thumb {
		background: white;
		height: 24px;
		width: 24px;
		border: none;
		border-radius: 13px;
	}
</style>
