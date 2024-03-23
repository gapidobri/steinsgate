<script>
	import Clock from '$lib/Clock.svelte';
	import Text from '$lib/Text.svelte';
</script>

<div class="flex h-screen flex-col items-center justify-center bg-black font-mono text-gray-300">
	<div class="flex grow flex-col items-center justify-center">
		<Clock />
		<Text />
	</div>
	<div class="flex w-full justify-end p-2">
		<span class="text-xs"></span>
			made by <a class="underline" href="https://l.gapi.me/anilist">gapi</a>
		</span>
	</div>
</div>
