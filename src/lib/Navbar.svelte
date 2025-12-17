<script lang="ts">
	import { X } from 'lucide-svelte';
</script>

<div class="fixed top-0 left-0 right-0 z-50">
	<!-- Top Banner -->
	<div class="bg-black text-white text-xs font-medium py-2.5 px-4 relative">
		<div class="flex justify-center items-center gap-2">
			<span>Pre-configured ERP connectors for seamless integration</span>
			<span class="opacity-70">→</span>
		</div>
		<button class="absolute right-4 top-1/2 -translate-y-1/2 text-white/60 hover:text-white">
			<X size={14} />
		</button>
	</div>

	<!-- Main Nav -->
	<nav class="bg-white/90 backdrop-blur-md border-b border-gray-200">
		<div class="max-w-[1400px] mx-auto px-6 h-16 flex items-center justify-between">
			<div class="flex items-center gap-8">
				<a href="/" class="flex items-center gap-2 text-black hover:opacity-80 transition-opacity">
					<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
						<path d="M12 4L4 8V16L12 20L20 16V8L12 4Z" fill="oklch(0.696 0.17 162.48)"/>
						<path d="M12 4V12M4 8L12 12M20 8L12 12M12 20V12M4 16L12 12M20 16L12 12" stroke="black" stroke-width="1"/>
					</svg>
					<span class="font-bold text-xl tracking-tight">Hivebuy</span>
				</a>

				<div class="hidden md:flex items-center gap-6 text-sm font-medium text-gray-600">
					<button class="hover:text-black flex items-center gap-1">
						Platform <span class="text-[10px]">▼</span>
					</button>
					<button class="hover:text-black flex items-center gap-1">
						Resources <span class="text-[10px]">▼</span>
					</button>
					<a href="#" class="hover:text-black">Customers</a>
					<a href="#" class="hover:text-black">Pricing</a>
				</div>
			</div>

			<div class="flex items-center gap-4">
				<a href="#" class="text-sm font-medium text-gray-600 hover:text-black">Sign in</a>
				<a href="#" class="bg-black text-white text-sm font-medium px-4 py-2 rounded-lg hover:bg-gray-800 transition-colors">
					Get started
				</a>
			</div>
		</div>
	</nav>
</div>
