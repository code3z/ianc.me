<script>
	import Card from '$lib/Card.svelte';
	export const prerender = true;
</script>

<svelte:head>
	<title>Ian's homepage</title>
</svelte:head>

<img src="/avatar.svg" alt="avatar" />
<h1>hey, I’m Ian</h1>
<h2>
	<a href="mailto:ian@ianc.me">ian@ianc.me</a>
</h2>
<div class="my-6">
	<p class="mb-3">
		I’m a 15yo web developer, designer, and entrepreneur (surprised I spelled that correctly).
	</p>

	<p>
		I’ve tried starting a startup and am currently doing an internship @ <a
			class="text-link"
			href="https://dots.community">dots.community.</a
		> I’m also a boy scout and do some other stuff. I designed and built this page, you can also check
		out some of my work below.
	</p>
</div>
<div class="grid auto-cols-min grid-flow-col gap-12">
	<Card
		title="@code3z"
		lightColor="#767C8A"
		darkColor="#5E636E"
		subtitle="github"
		icon="/github.svg"
		url="https://github.com/code3z"
		target="_blank"
	/>
	<Card
		title="Dots (YC S21)"
		lightColor="#FF7F60"
		darkColor="#8E320B"
		subtitle="internship"
		icon="/dots.svg"
		url="/todo"
	/>
	<Card
		title="Shareweave"
		lightColor="#0BCAF4"
		darkColor="#298CA1"
		subtitle="project"
		icon="/shareweave-padded-round.svg"
		url="/todo"
	/>
</div>
