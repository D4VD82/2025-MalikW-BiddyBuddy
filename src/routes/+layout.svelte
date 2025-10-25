<script lang="ts">
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children?.()}

<nav class="nav_bar">
	<a href="/dirty"> Dirty</a>
	<a href="/annoying"> Annoying</a>
	<a href="/home"> Home</a>
	<a href="/hungry"> Hungry</a>
	<a href="/ill"> Ill</a>
	<a href="/neglected"> Neglected</a>
	<a href="/sleepy"> Sleepy</a>
</nav>

<style>
.nav_bar{
	display:flex;
	justify-content: space-around;
}

.nav_bar > * {
	display: flex;
	justify-content: center;
	width: 80px;
	height:20px;
	border: 2px solid black;
}
</style>
