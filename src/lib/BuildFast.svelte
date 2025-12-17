<script lang="ts">
	import { Mail, Calendar, Database, Activity, Search, Bell, CheckSquare, BarChart2, Zap, MoreHorizontal, Filter, RefreshCw, Plus } from 'lucide-svelte';
</script>

<section class="max-w-[1200px] mx-auto px-6 py-20 text-center">
	<div class="max-w-3xl mx-auto mb-12">
		<h2 class="text-4xl font-serif text-gray-900 mb-6">
			Set up in minutes. <span class="text-gray-500 font-sans text-xl font-normal block mt-4">Forget months of implementation. Hivebuy connects to your ERP system instantly, importing your vendors, budgets, and approval chains automatically.</span>
		</h2>
		<button class="mt-8 px-5 py-2.5 bg-black text-white rounded-lg text-sm font-medium hover:bg-gray-800 transition-colors">
			Get started
		</button>
	</div>

	<!-- Tabs -->
	<div class="flex justify-center gap-4 mb-12">
		<button class="flex items-center gap-2 px-4 py-2 bg-white border border-gray-200 rounded-full text-xs font-medium text-gray-900 shadow-sm hover:bg-gray-50">
			<Database size={14} /> ERP Integration
		</button>
		<button class="flex items-center gap-2 px-4 py-2 bg-white border border-gray-200 rounded-full text-xs font-medium text-gray-500 hover:text-gray-900 hover:bg-gray-50 transition-colors">
			<Mail size={14} /> Vendor Import
		</button>
		<button class="flex items-center gap-2 px-4 py-2 bg-white border border-gray-200 rounded-full text-xs font-medium text-gray-500 hover:text-gray-900 hover:bg-gray-50 transition-colors">
			<Activity size={14} /> Budget Setup
		</button>
		<button class="flex items-center gap-2 px-4 py-2 bg-white border border-gray-200 rounded-full text-xs font-medium text-gray-500 hover:text-gray-900 hover:bg-gray-50 transition-colors">
			<CheckSquare size={14} /> Approval Chains
		</button>
	</div>

	<!-- UI Preview -->
	<div class="relative bg-white rounded-xl border border-gray-200 shadow-xl overflow-hidden text-left max-w-5xl mx-auto">
		<!-- Header -->
		<div class="h-14 border-b border-gray-200 flex items-center justify-between px-6 bg-white">
			<div class="flex items-center gap-4">
				<div class="w-8 h-8 rounded bg-gray-200 flex items-center justify-center text-sm font-bold text-gray-700">
					S
				</div>
				<div>
					<div class="text-sm font-semibold text-gray-900">Siemens AG</div>
					<div class="text-xs text-gray-500">Preferred Vendor - IT Equipment</div>
				</div>
			</div>
			<div class="flex items-center gap-3">
				<button class="text-gray-400 hover:text-gray-600"><Search size={16} /></button>
				<button class="text-gray-400 hover:text-gray-600"><Bell size={16} /></button>
				<button class="text-gray-400 hover:text-gray-600"><MoreHorizontal size={16} /></button>
			</div>
		</div>

		<div class="flex h-[500px]">
			<!-- Sidebar -->
			<div class="w-64 border-r border-gray-200 bg-gray-50/30 p-4 flex flex-col gap-1">
				<div class="text-[11px] font-medium text-gray-400 mb-2 uppercase tracking-wider">Details</div>
				
				<div class="grid grid-cols-[20px_1fr] gap-2 text-xs mb-4">
					<div class="text-gray-400"><Mail size={14} /></div>
					<div class="text-gray-900 truncate">procurement@siemens.com</div>
					
					<div class="text-gray-400"><Calendar size={14} /></div>
					<div class="text-gray-900">Last order 5 days ago</div>
					
					<div class="text-gray-400"><Database size={14} /></div>
					<div class="text-gray-900">€2.4M annual spend</div>
				</div>

				<div class="text-[11px] font-medium text-gray-400 mb-2 uppercase tracking-wider mt-4">Categories</div>
				<div class="flex items-center gap-2 text-xs text-gray-700 bg-white border border-gray-200 p-2 rounded shadow-sm">
					<div class="w-2 h-2 rounded-full" style="background: oklch(0.696 0.17 162.48)"></div> IT Equipment
				</div>
			</div>

			<!-- Main Content -->
			<div class="flex-1 bg-white p-6 overflow-y-auto">
				<div class="flex items-center justify-between mb-6">
					<h3 class="text-sm font-semibold text-gray-900 flex items-center gap-2">
						<Activity size={16} /> Recent Activity
					</h3>
					<button class="text-xs font-medium" style="color: oklch(0.696 0.17 162.48)">+ Add purchase order</button>
				</div>

				<!-- Highlight Card -->
				<div class="border rounded-lg p-4 mb-8" style="background: oklch(0.979 0.021 166.113); border-color: oklch(0.905 0.093 164.15)">
					<p class="text-sm text-gray-700 leading-relaxed">
						Siemens has been added as a preferred vendor for IT Equipment. Payment terms: Net 30. Average delivery time: 5-7 business days.
					</p>
					<div class="flex items-center gap-2 mt-3">
						<div class="w-5 h-5 rounded flex items-center justify-center text-[10px] text-white font-medium" style="background: oklch(0.696 0.17 162.48)">✓</div>
						<span class="text-xs text-gray-500">Auto-imported from SAP</span>
					</div>
				</div>

				<!-- Timeline -->
				<div class="relative pl-4 border-l border-gray-200 space-y-8">
					<!-- Event 1 -->
					<div class="relative">
						<div class="absolute -left-[21px] top-0 w-3 h-3 rounded-full bg-gray-200 border-2 border-white"></div>
						<div class="flex items-start justify-between">
							<div>
								<div class="text-sm font-medium text-gray-900">Purchase Order: PO-2024-0342</div>
								<p class="text-xs text-gray-500 mt-1">IT Equipment - €12,450 - Approved by Bettina Fischer</p>
							</div>
							<span class="text-xs text-gray-400">5 days ago</span>
						</div>
					</div>

					<!-- Event 2 -->
					<div class="relative">
						<div class="absolute -left-[21px] top-0 w-3 h-3 rounded-full border-2 border-white" style="background: oklch(0.696 0.17 162.48)"></div>
						<div class="flex items-start justify-between">
							<div>
								<div class="text-sm font-medium text-gray-900">Contract Renewal</div>
								<div class="flex items-center gap-2 mt-1">
									<span class="text-xs text-gray-500">Annual agreement renewed - €2.4M</span>
								</div>
							</div>
							<span class="text-xs text-gray-400">12 days ago</span>
						</div>
					</div>
					
					<!-- Event 3 -->
					<div class="relative">
						<div class="absolute -left-[21px] top-0 w-3 h-3 rounded-full bg-gray-200 border-2 border-white"></div>
						<div class="flex items-start justify-between">
							<div>
								<div class="text-sm font-medium text-gray-900">Stefan Kiehne added Siemens to "Preferred Vendors"</div>
							</div>
							<span class="text-xs text-gray-400">30 days ago</span>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</section>
