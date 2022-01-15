<script>
	import '../app.css';
	import Nav from '../components/nav.svelte';
	import Footer from '../components/footer.svelte';
</script>

<div class="flex flex-col bg-gradient-to-b from-green-400 to-orange-400 h-screen">
	<div><Nav /></div>
	<div class="mb-auto"><slot /></div>
	<div><Footer /></div>
</div>
