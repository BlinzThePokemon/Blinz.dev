<script>
	import '../app.css';
	let { children } = $props();
</script>

{@render children()}
<nav class="bg-white shadow-md">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
        <div class="flex h-16 items-center justify-center">
            <div class="hidden space-x-4 sm:flex">
				<a href="#" class="rounded-md px-3 py-2 text-sm font-medium hover:bg-gray-500 hover:text-white active:bg-gray-900 active:text-white">Home</a>
				<a href="#" class="rounded-md px-3 py-2 text-sm font-medium hover:bg-gray-500 hover:text-white active:bg-gray-900 active:text-white">Projects</a>
				<a href="#" class="rounded-md px-3 py-2 text-sm font-medium hover:bg-gray-500 hover:text-white active:bg-gray-900 active:text-white">Contact Me</a>
			</div>
        </div>
    </div>
</nav>
