<script lang="ts">
	import './layout.css';
	
</script>

<nav class="bg-blue-200 fixed w-full z-20 top-0 start-0">
	<div class="flex flex-wrap items-center justify-between mx-auto p-4">
		<h2 class="text-left font-bold">lipu pi kama sona</h2>
	</div>
	
</nav>

<main class="p-20 bg-blue-100/60 h-screen">
	<slot />
</main>
