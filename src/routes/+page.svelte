<script>
	import Card from '$lib/Card.svelte';
	export const prerender = true;
</script>

<svelte:head>
	<title>Ian's homepage</title>
	<meta property="og:title" content="Ian's homepage" />
	<meta property="og:type" content="video.movie" />
	<meta property="og:url" content="https://ianc.me/" />
	<meta property="og:image" content="/avatar.svg" />
	<meta
		name="description"
		property="og:description"
		content="My homepage. I'm a 15yo web developer, designer, and entrepreneur."
	/>
</svelte:head>

<img src="/avatar.svg" alt="avatar" class="hover:-rotate-12 transition-all duration-150" />
<h1 class="mb-1">hey, i’m ian</h1>
<h2>
	<a class="no-link-style" href="mailto:ian@ianc.me">ian@ianc.me</a>
</h2>
<div class="my-6 text-lg text-gray-200">
	<p class="mb-3">
		I’m a 15yo web developer, designer, and entrepreneur (and always trying to learn more).
	</p>

	<p>
		I’ve tried starting a startup, which led to an internship @ <a
			class="text-link"
			href="https://dots.community">dots.community.</a
		>
		(a company I had previously wanted to compete against). Right now, I'm working as a software engineer
		at <a class="text-link" href="https://thirdbuy.com">thirdbuy.</a> I’m also a boy scout and do some
		other stuff. You can check out some of my work below - in addition to designing this page, of course
		:)
	</p>
</div>
<div class="grid grid-cols-[repeat(auto-fit,minmax(16rem,1fr))] gap-12">
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
		url="/dots"
	/>
	<Card
		title="Dots Email Digest"
		lightColor="rgb(19, 87, 217)"
		darkColor="#04008e"
		subtitle="project"
		icon="✉️"
		url="/todo"
	/>
	<Card
		title="Shareweave"
		lightColor="#0BCAF4"
		darkColor="#298CA1"
		subtitle="project"
		icon="/shareweave-padded-round.svg"
		url="/shareweave"
	/>

	<Card
		title="Thirdbuy"
		lightColor="rgb(175, 87, 200)"
		darkColor="#7D37EE"
		subtitle="job"
		icon="/thirdbuy-icon.png"
		url="/thirdbuy"
		target="_blank"
	/>
	<Card
		title="read.cv/ic"
		lightColor="rgb(0, 172, 132)"
		darkColor="rgb(26, 70, 0)"
		subtitle="resume"
		icon="/readcv.png"
		url="https://read.cv/ic"
		target="_blank"
	/>
</div>
