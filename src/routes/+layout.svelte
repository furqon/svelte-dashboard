<script>
	import '../app.css';

	import Navbar from '$lib/components/navbar.svelte';
	import Sidebar from '$lib/components/sidebar.svelte';
	import Footer from '$lib/components/footer.svelte';
</script>

<div>
	<Navbar />
	<div class="flex overflow-hidden bg-white pt-16">
		<Sidebar />
		<div id="main-content" class="h-full w-full bg-gray-50 relative overflow-y-auto lg:ml-64">
			<main><div class="pt-6 px-4"><slot /></div></main>

			<Footer />
		</div>
	</div>
</div>
