<script>
	import { onMount } from 'svelte';

	onMount(() => {
		const btn = document.querySelector('button');
		const menu = document.querySelector('.mobile-menu');

		btn.addEventListener('click', () => {
			menu.classList.toggle('hidden');
		});
	});
</script>

<nav>
	<div class="flex justify-between items-center bg-green-700 text-white font-bold space-x-3">
		<div class="flex items-center p-3">
			<span>
				<svg
					xmlns="http://www.w3.org/2000/svg"
					class="h-12 w-12"
					fill="none"
					viewBox="0 0 24 24"
					stroke="currentColor">
					<path
						stroke-linecap="round"
						stroke-linejoin="round"
						stroke-width="2"
						d="M17 9V7a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2m2 4h10a2 2 0 002-2v-6a2 2 0 00-2-2H9a2 2 0 00-2 2v6a2 2 0 002 2zm7-5a2 2 0 11-4 0 2 2 0 014 0z" />
				</svg></span>
			<span class="text-2xl"> Money Maker</span>
		</div>
		<div class="hidden md:block p-4 text-xl">
			<a href="/" class="hover:bg-orange-700">Home</a>
			<a href="/about" class="hover:bg-orange-700">About</a>
			<a href="/contact" class="hover:bg-orange-700">Contact</a>
		</div>
		<div class="block md:hidden p-4">
			<button>
				<svg
					xmlns="http://www.w3.org/2000/svg"
					class="h-8 w-8"
					fill="none"
					viewBox="0 0 24 24"
					stroke="currentColor">
					<path
						stroke-linecap="round"
						stroke-linejoin="round"
						stroke-width="2"
						d="M4 6h16M4 12h16M4 18h16" />
				</svg>
			</button>
		</div>
	</div>
	<div
		class="flex flex-col mobile-menu md:hidden hidden text-white bg-green-700 font-bold text-xl">
		<a href="/" class="hover:text-orange-700 p-4">Home</a>
		<a href="/about" class="hover:text-orange-700 p-4">About</a>
		<a href="/contact" class="hover:text-orange-700 p-4">Contact</a>
	</div>
</nav>
