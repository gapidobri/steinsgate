<script lang="ts">
	import Typewriter from 'svelte-typewriter';

	const d = 2000;
</script>

<div class="mt-8 flex flex-col items-center text-center">
	<div class="h-6">
		<Typewriter interval={50} delay={d}>Decieve your other self.</Typewriter>
	</div>
	<div class="mt-3 h-6">
		<Typewriter interval={50} delay={d + 2000}>Decieve the world.</Typewriter>
	</div>
	<div class="mt-1 h-6">
		<Typewriter interval={50} delay={d + 4000}>
			That is what you must do to reach Steins Gate.
		</Typewriter>
	</div>
	<div class="mt-3 h-6">
		<Typewriter interval={50} delay={d + 7000}>Good luck.</Typewriter>
	</div>
	<div class="mt-8 flex h-7 space-x-2 text-lg font-bold">
		<Typewriter interval={50} delay={d + 8500}>El.</Typewriter>
		<Typewriter interval={50} delay={d + 9500}>Psy.</Typewriter>
		<Typewriter interval={50} delay={d + 10500}>Congroo.</Typewriter>
	</div>
</div>
