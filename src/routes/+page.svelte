<script>
	import WalletConnect from '$lib/WalletConnect.svelte';
	import LocalSign from '$lib/LocalSign.svelte';

	/** @type {Web3Props} */
	export let web3Props;
</script>

{#if !web3Props?.account}
	<div class="grid h-screen place-items-center">
		<WalletConnect bind:web3Props />
	</div>
{:else}
	<LocalSign bind:web3Props />
{/if}
