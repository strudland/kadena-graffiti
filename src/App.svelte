<script lang="ts">
	import Header from './Header.svelte';
	import Footer from './Footer.svelte';
	import Graffiti from './Graffiti.svelte';

	export let name: string;

	
</script>

<appContainer>
	<Header />
	<main>
		<Graffiti />	
	</main>
	<Footer />
</appContainer>


<style>
	appContainer {
		height: 100%;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: space-between;
	}

	main {
		width: 100%;
		flex-grow: 1;
	}
</style>