<script lang="ts">
	import { User, Briefcase, Building2, Plus, MoreHorizontal } from 'lucide-svelte';
</script>

<section class="max-w-[1200px] mx-auto px-6 py-20">
	<div class="text-center max-w-3xl mx-auto mb-20">
		<h2 class="text-4xl font-serif text-gray-900 mb-6">
			Flexible procurement data model. <span class="text-gray-500 font-sans text-xl font-normal block mt-4">Hivebuy's powerful data model adapts to your procurement processes, not the other way around. Your workflows — perfectly reflected in the system.</span>
		</h2>
		<button class="mt-8 px-4 py-2 bg-white border border-gray-200 rounded-full text-sm font-medium hover:border-gray-300 transition-colors">
			Explore our data model
		</button>
	</div>

	<!-- Data Model Visual -->
	<div class="relative bg-gray-50/50 rounded-xl p-10 md:p-20 border border-gray-100 overflow-hidden">
		<!-- Background Grid -->
		<div class="absolute inset-0" style="background-image: radial-gradient(#e5e7eb 1px, transparent 1px); background-size: 20px 20px; opacity: 0.5;"></div>

		<!-- Top Filters -->
		<div class="flex justify-center gap-2 mb-16 relative z-10">
			<button class="px-3 py-1 bg-white border border-gray-200 rounded-full text-xs font-medium shadow-sm">Manufacturing</button>
			<button class="px-3 py-1 bg-white border border-gray-200 rounded-full text-xs font-medium shadow-sm">Retail</button>
			<button class="px-3 py-1 bg-white border border-gray-200 rounded-full text-xs font-medium shadow-sm">Services</button>
			<button class="px-3 py-1 bg-white border border-gray-200 rounded-full text-xs font-medium shadow-sm">Construction</button>
		</div>

		<!-- Objects Diagram -->
		<div class="relative max-w-4xl mx-auto h-[500px]">
			<!-- Connecting Lines (SVG) -->
			<svg class="absolute inset-0 w-full h-full pointer-events-none z-0">
				<!-- User to Person -->
				<path d="M 200 150 C 200 200, 250 250, 300 300" fill="none" stroke="#e5e7eb" stroke-width="2" stroke-dasharray="4 4" />
				<!-- Person to Deal -->
				<path d="M 450 300 C 500 250, 550 200, 600 150" fill="none" stroke="#e5e7eb" stroke-width="2" stroke-dasharray="4 4" />
				<!-- Person to Add Object -->
				<path d="M 450 350 C 500 350, 550 350, 600 350" fill="none" stroke="#e5e7eb" stroke-width="2" stroke-dasharray="4 4" />
			</svg>

			<!-- Vendor Object -->
			<div class="absolute top-10 left-10 w-64 bg-white rounded-lg border border-gray-200 shadow-sm z-10">
				<div class="p-3 border-b border-gray-100 flex items-center justify-between bg-gray-50/50 rounded-t-lg">
					<div class="flex items-center gap-2">
						<div class="w-6 h-6 rounded flex items-center justify-center" style="background: oklch(0.95 0.052 163.051); color: oklch(0.696 0.17 162.48)">
							<Building2 size={14} />
						</div>
						<span class="text-sm font-semibold text-gray-900">Vendor</span>
					</div>
					<span class="text-[10px] text-gray-400 bg-gray-100 px-1.5 py-0.5 rounded">Standard</span>
				</div>
				<div class="p-3 space-y-2">
					<div class="flex items-center gap-2 text-xs text-gray-600">
						<div class="w-4 h-4 flex items-center justify-center text-gray-400">Aa</div>
						<span>Vendor name</span>
					</div>
					<div class="flex items-center gap-2 text-xs text-gray-600">
						<div class="w-4 h-4 flex items-center justify-center text-gray-400">€</div>
						<span>Total spend</span>
					</div>
					<div class="flex items-center gap-2 text-xs text-gray-600">
						<div class="w-4 h-4 flex items-center justify-center text-gray-400">≡</div>
						<span>Category</span>
					</div>
					<div class="text-[10px] text-gray-400 pl-6">+ 6 More Attributes</div>
				</div>
			</div>

			<!-- Budget Object -->
			<div class="absolute top-10 right-10 w-64 bg-white rounded-lg border border-gray-200 shadow-sm z-10">
				<div class="p-3 border-b border-gray-100 flex items-center justify-between bg-gray-50/50 rounded-t-lg">
					<div class="flex items-center gap-2">
						<div class="w-6 h-6 rounded bg-purple-100 flex items-center justify-center text-purple-600">
							<Briefcase size={14} />
						</div>
						<span class="text-sm font-semibold text-gray-900">Budget</span>
					</div>
					<span class="text-[10px] text-gray-400 bg-gray-100 px-1.5 py-0.5 rounded">Standard</span>
				</div>
				<div class="p-3 space-y-2">
					<div class="flex items-center gap-2 text-xs text-gray-600">
						<div class="w-4 h-4 flex items-center justify-center text-gray-400">Aa</div>
						<span>Department</span>
					</div>
					<div class="flex items-center gap-2 text-xs text-gray-600">
						<div class="w-4 h-4 flex items-center justify-center text-gray-400">€</div>
						<span>Allocated amount</span>
					</div>
					<div class="flex items-center gap-2 text-xs text-gray-600">
						<div class="w-4 h-4 flex items-center justify-center text-gray-400">%</div>
						<span>Utilization</span>
					</div>
					<div class="text-[10px] text-gray-400 pl-6">+ 4 More Attributes</div>
				</div>
			</div>

			<!-- Purchase Order Object (Center) -->
			<div class="absolute top-60 left-1/2 -translate-x-full -ml-4 w-64 bg-white rounded-lg border border-gray-200 shadow-sm z-10">
				<div class="p-3 border-b border-gray-100 flex items-center justify-between bg-gray-50/50 rounded-t-lg">
					<div class="flex items-center gap-2">
						<div class="w-6 h-6 rounded bg-blue-100 flex items-center justify-center text-blue-600">
							<User size={14} />
						</div>
						<span class="text-sm font-semibold text-gray-900">Purchase Order</span>
					</div>
					<span class="text-[10px] text-gray-400 bg-gray-100 px-1.5 py-0.5 rounded">Standard</span>
				</div>
				<div class="p-3 space-y-2">
					<div class="flex items-center gap-2 text-xs text-gray-600">
						<div class="w-4 h-4 flex items-center justify-center text-gray-400">#</div>
						<span>PO Number</span>
					</div>
					<div class="flex items-center gap-2 text-xs text-gray-600">
						<div class="w-4 h-4 flex items-center justify-center text-gray-400">€</div>
						<span>Amount</span>
					</div>
					<div class="flex items-center gap-2 text-xs text-gray-600">
						<div class="w-4 h-4 flex items-center justify-center text-gray-400">✓</div>
						<span>Approval status</span>
					</div>
					<div class="text-[10px] text-gray-400 pl-6">+ 8 More Attributes</div>
				</div>
			</div>

			<!-- Add Object (Placeholder) -->
			<div class="absolute top-60 left-1/2 ml-4 w-64 h-40 border-2 border-dashed border-blue-200 rounded-lg flex items-center justify-center bg-blue-50/30 z-10">
				<div class="flex items-center gap-2 text-blue-500 font-medium text-sm">
					<Plus size={16} /> Add object
				</div>
			</div>
		</div>

		<!-- Table View at Bottom -->
		<div class="mt-10 bg-white border border-gray-200 rounded-lg shadow-sm overflow-hidden max-w-4xl mx-auto">
			<div class="grid grid-cols-4 gap-4 p-3 border-b border-gray-100 bg-gray-50 text-[11px] font-medium text-gray-500">
				<div class="flex items-center gap-2"><User size={12} /> Purchase Order</div>
				<div class="flex items-center gap-2"><div class="w-3 h-3 flex items-center justify-center">#</div> PO Number</div>
				<div class="flex items-center gap-2"><div class="w-3 h-3 flex items-center justify-center">€</div> Amount</div>
				<div class="flex items-center gap-2"><div class="w-3 h-3 flex items-center justify-center">✓</div> Status</div>
			</div>
			<!-- Row 1 -->
			<div class="grid grid-cols-4 gap-4 p-3 border-b border-gray-50 text-xs hover:bg-gray-50">
				<div class="flex items-center gap-2"><div class="w-5 h-5 rounded bg-gray-100 flex items-center justify-center text-[10px] font-medium">IT</div> IT Equipment</div>
				<div class="font-mono text-gray-500 text-[10px]">PO-2024-0342</div>
				<div class="font-medium">€12,450</div>
				<div><span class="bg-green-100 text-green-700 px-1.5 py-0.5 rounded text-[10px]">Approved</span></div>
			</div>
			<!-- Row 2 -->
			<div class="grid grid-cols-4 gap-4 p-3 border-b border-gray-50 text-xs hover:bg-gray-50">
				<div class="flex items-center gap-2"><div class="w-5 h-5 rounded bg-gray-100 flex items-center justify-center text-[10px] font-medium">MK</div> Marketing Materials</div>
				<div class="font-mono text-gray-500 text-[10px]">PO-2024-0341</div>
				<div class="font-medium">€8,200</div>
				<div><span class="bg-yellow-100 text-yellow-700 px-1.5 py-0.5 rounded text-[10px]">Pending</span></div>
			</div>
			<!-- Row 3 -->
			<div class="grid grid-cols-4 gap-4 p-3 border-b border-gray-50 text-xs hover:bg-gray-50">
				<div class="flex items-center gap-2"><div class="w-5 h-5 rounded bg-gray-100 flex items-center justify-center text-[10px] font-medium">OP</div> Office Supplies</div>
				<div class="font-mono text-gray-500 text-[10px]">PO-2024-0340</div>
				<div class="font-medium">€3,750</div>
				<div><span class="bg-green-100 text-green-700 px-1.5 py-0.5 rounded text-[10px]">Approved</span></div>
			</div>
			<!-- Row 4 -->
			<div class="grid grid-cols-4 gap-4 p-3 text-xs hover:bg-gray-50">
				<div class="flex items-center gap-2"><div class="w-5 h-5 rounded bg-gray-100 flex items-center justify-center text-[10px] font-medium">HR</div> Training Services</div>
				<div class="font-mono text-gray-500 text-[10px]">PO-2024-0339</div>
				<div class="font-medium">€15,600</div>
				<div><span class="bg-blue-100 text-blue-700 px-1.5 py-0.5 rounded text-[10px]">In Review</span></div>
			</div>
		</div>
	</div>
</section>
