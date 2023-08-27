<script>
	import Header from './Header.svelte';
	import CardList from './CardList.svelte';
	export let isMonthly;

	function handleSwitch(event) {
		// console.log(event.detail.isMonthly);
		isMonthly = event.detail.isMonthly === '1';
	}
</script>

<Header on:handleSwitch={handleSwitch} />

<CardList {isMonthly} />
