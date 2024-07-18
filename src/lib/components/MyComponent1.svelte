<script lang="ts">
	type ComponentProps = {
		disabled?: boolean;
		label: string;
	};

	let { disabled = false, label }: ComponentProps = $props();
</script>

<div>
	{#if disabled}
		<button disabled>{label}</button>
	{:else}
		<button>{label}</button>
	{/if}
</div>
