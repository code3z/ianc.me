<script lang="ts">
	export let title: string;
	export let subtitle: string;
	export let icon: string;
	export let lightColor: string;
	export let darkColor: string;
	export let url: string;
	export let target: string = '';

	const iconIsEmoji = icon.match(/\p{Emoji}/gu)?.length === 1 ? true : false;
</script>

<a
	href={url}
	{target}
	style:background={`linear-gradient(302.27deg, ${darkColor} 0.99%, ${lightColor} 100%)`}
	class="grid grid-rows-[8rem_1rem_auto] p-6 rounded-3xl w-full shadow-lg hover:scale-90 transition-transform duration-300"
>
	<div>
		{#if iconIsEmoji}
			<span class="text-[4rem] leading-[4rem]">{icon}</span>
		{:else}
			<img src={icon} class="h-16" alt="icon" />
		{/if}
	</div>
	<small class="text-sm opacity-60 font-semibold uppercase">{subtitle}</small>
	<p class="text-2xl font-bold mt-2 truncate">{title}</p>
</a>
