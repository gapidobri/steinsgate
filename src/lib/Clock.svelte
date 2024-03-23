<script lang="ts">
	import n0 from '$lib/assets/numbers/0.png';
	import n1 from '$lib/assets/numbers/1.png';
	import n2 from '$lib/assets/numbers/2.png';
	import n3 from '$lib/assets/numbers/3.png';
	import n4 from '$lib/assets/numbers/4.png';
	import n5 from '$lib/assets/numbers/5.png';
	import n6 from '$lib/assets/numbers/6.png';
	import n7 from '$lib/assets/numbers/7.png';
	import n8 from '$lib/assets/numbers/8.png';
	import n9 from '$lib/assets/numbers/9.png';
	import dot from '$lib/assets/numbers/p.png';
	import rnd1 from '$lib/assets/numbers/random1.gif';
	import rnd2 from '$lib/assets/numbers/random2.gif';
	import { onMount } from 'svelte';

	const numbers = [n0, n1, n2, n3, n4, n5, n6, n7, n8, n9];

	const display = new Array(8).fill('').map(() => (Math.random() < 0.5 ? rnd1 : rnd2));
	display[1] = dot;

	onMount(() => {
		for (let i = 0; i < display.length; i++) {
			if (i === 1) continue;
			setTimeout(() => {
				display[i] = numbers[Math.floor(Math.random() * numbers.length)];
			}, Math.random() * 2000);
		}
	});
</script>

<div class="flex">
	{#each display as digit}
		<img src={digit} class="w-10" alt="digit" />
	{/each}
</div>
