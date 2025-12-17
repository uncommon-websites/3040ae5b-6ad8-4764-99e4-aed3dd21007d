<script lang="ts">
	import { ArrowRight, ChevronDown, Search, Bell, CheckSquare, Mail, BarChart2, Zap, Layout, Users, Briefcase, Building2, Plus, MoreHorizontal, Filter, RefreshCw, Download } from 'lucide-svelte';
</script>

<section class="pt-40 pb-20 px-6 text-center max-w-[1400px] mx-auto">
	<a href="#" class="inline-flex items-center gap-2 text-xs font-medium text-gray-500 hover:text-black mb-8 border border-gray-200 rounded-full px-3 py-1 bg-white hover:border-gray-300 transition-colors">
		Trusted by 10,000+ German SMEs
		<ArrowRight size={12} />
	</a>

	<h1 class="text-[56px] leading-[1.1] font-serif tracking-tight text-gray-900 mb-6 max-w-4xl mx-auto">
		Indirect Procurement on Autopilot
	</h1>

	<p class="text-lg text-gray-500 mb-10 max-w-xl mx-auto text-balance">
		Automate requests, approvals, and purchasing with zero operational friction.
	</p>

	<div class="flex items-center justify-center gap-4 mb-20">
		<a href="#" class="bg-black text-white text-sm font-medium px-5 py-2.5 rounded-lg hover:bg-gray-800 transition-colors">
			Get started
		</a>
		<a href="#" class="text-sm font-medium text-gray-600 hover:text-black border border-gray-200 px-5 py-2.5 rounded-lg hover:border-gray-300 transition-colors">
			Book a demo
		</a>
	</div>

	<!-- Dashboard Preview -->
	<div class="relative rounded-xl overflow-hidden shadow-2xl border border-gray-200 bg-white text-left mx-auto max-w-[1200px]">
		<!-- Tabs -->
		<div class="flex border-b border-gray-200 bg-gray-50/50">
			<button class="px-8 py-3 text-xs font-medium text-gray-500 hover:text-black border-b-2 border-transparent">Purchase Orders</button>
			<button class="px-8 py-3 text-xs font-medium text-gray-500 hover:text-black border-b-2 border-transparent">Approvals</button>
			<button class="px-8 py-3 text-xs font-medium text-black border-b-2 border-black bg-white">Budget Tracking</button>
			<button class="px-8 py-3 text-xs font-medium text-gray-500 hover:text-black border-b-2 border-transparent">Vendors</button>
		</div>

		<!-- UI Container -->
		<div class="flex h-[600px] bg-white">
			<!-- Sidebar -->
			<div class="w-[240px] border-r border-gray-200 flex flex-col text-[13px] text-gray-600">
				<div class="p-3 flex items-center gap-2 font-medium text-black border-b border-gray-100">
					<div class="w-5 h-5 bg-black rounded flex items-center justify-center text-white text-[10px]">M</div>
					Müller GmbH
					<ChevronDown size={14} class="ml-auto opacity-50" />
				</div>
				
				<div class="p-2 space-y-0.5">
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<Search size={14} /> Quick search
						<div class="ml-auto text-[10px] border border-gray-200 rounded px-1">⌘K</div>
					</div>
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<Bell size={14} /> Approvals
					</div>
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<CheckSquare size={14} /> Purchase Orders
					</div>
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<Mail size={14} /> Invoices
					</div>
					<div class="flex items-center gap-2 px-2 py-1.5 bg-gray-100 text-black font-medium rounded cursor-pointer">
						<BarChart2 size={14} /> Budget Reports
					</div>
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<Zap size={14} /> Workflows
					</div>
				</div>

				<div class="mt-2 px-4 text-[11px] font-medium text-gray-400">Management</div>
				<div class="p-2 space-y-0.5">
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<Building2 size={14} class="text-blue-500" /> Vendors
					</div>
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<Users size={14} class="text-green-500" /> Departments
					</div>
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<Briefcase size={14} class="text-orange-500" /> Budgets
					</div>
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<Layout size={14} class="text-purple-500" /> Categories
					</div>
				</div>
			</div>

			<!-- Main Content -->
			<div class="flex-1 flex flex-col bg-gray-50/30">
				<!-- Header -->
				<div class="h-14 border-b border-gray-200 flex items-center justify-between px-6 bg-white">
					<div class="flex items-center gap-2 text-sm text-gray-500">
						<BarChart2 size={16} />
						<span>Budget Reports</span>
						<span class="text-gray-300">/</span>
						<span class="text-black font-medium">Q1 Spending Overview</span>
					</div>
					<div class="flex items-center gap-3">
						<div class="flex -space-x-2">
							<div class="w-6 h-6 rounded-full bg-blue-100 border-2 border-white flex items-center justify-center text-[10px]">BF</div>
							<div class="w-6 h-6 rounded-full bg-green-100 border-2 border-white flex items-center justify-center text-[10px]">SK</div>
						</div>
						<button class="text-xs font-medium text-gray-600 hover:text-black flex items-center gap-1">
							Export
						</button>
					</div>
				</div>

				<!-- Dashboard Content -->
				<div class="p-6 overflow-hidden">
					<div class="mb-6 flex items-center justify-between">
						<div>
							<h2 class="text-lg font-semibold text-gray-900">Q1 Spending Overview</h2>
							<p class="text-sm text-gray-500">Real-time budget tracking across departments, vendors, and categories.</p>
						</div>
						<div class="flex items-center gap-2">
							<button class="text-xs font-medium text-gray-500 hover:text-black flex items-center gap-1 px-2 py-1">
								<RefreshCw size={12} /> Refresh data
							</button>
							<button class="bg-blue-600 text-white text-xs font-medium px-3 py-1.5 rounded-md hover:bg-blue-700 flex items-center gap-1">
								<Plus size={12} /> New budget
							</button>
						</div>
					</div>

					<div class="grid grid-cols-5 gap-6 h-full">
						<!-- Chart 1: Budget spending -->
						<div class="col-span-3 bg-white rounded-lg border border-gray-200 p-4 shadow-sm">
							<div class="flex items-center justify-between mb-4">
								<h3 class="text-sm font-medium text-gray-900">Department spending by category</h3>
								<MoreHorizontal size={14} class="text-gray-400" />
							</div>
							<div class="flex items-center gap-4 text-[10px] text-gray-500 mb-4">
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full" style="background: oklch(0.696 0.17 162.48)"></div> IT</div>
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full" style="background: oklch(0.596 0.145 163.225)"></div> Marketing</div>
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full" style="background: oklch(0.508 0.118 165.612)"></div> Operations</div>
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full" style="background: oklch(0.432 0.095 166.913)"></div> HR</div>
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full" style="background: oklch(0.378 0.077 168.94)"></div> Finance</div>
							</div>
							
							<!-- Mock Bar Chart -->
							<div class="relative h-[250px] w-full mt-8">
								<!-- Y Axis Labels -->
								<div class="absolute left-0 top-0 bottom-0 w-8 flex flex-col justify-between text-[10px] text-gray-400 text-right pr-2">
									<span>€ 280k</span>
									<span>€ 240k</span>
									<span>€ 200k</span>
									<span>€ 160k</span>
									<span>€ 120k</span>
									<span>€ 80k</span>
									<span>€ 40k</span>
								</div>
								<!-- Bars -->
								<div class="ml-10 h-full flex items-end justify-between px-4 border-l border-b border-gray-100">
									<!-- January -->
									<div class="w-8 flex flex-col gap-0.5 items-center group relative">
										<div class="w-full h-8 rounded-t-sm" style="background: oklch(0.845 0.143 164.978)"></div>
										<div class="w-full h-12" style="background: oklch(0.765 0.177 163.223)"></div>
										<div class="w-full h-16" style="background: oklch(0.696 0.17 162.48)"></div>
										<div class="absolute -bottom-6 text-[10px] text-gray-500">Jan</div>
									</div>
									<!-- February -->
									<div class="w-8 flex flex-col gap-0.5 items-center relative">
										<div class="w-full h-10 rounded-t-sm" style="background: oklch(0.765 0.177 163.223)"></div>
										<div class="w-full h-16" style="background: oklch(0.696 0.17 162.48)"></div>
										<div class="w-full h-24" style="background: oklch(0.596 0.145 163.225)"></div>
										<div class="absolute -bottom-6 text-[10px] text-gray-500">Feb</div>
										
										<!-- Tooltip Mock -->
										<div class="absolute bottom-full mb-2 left-1/2 -translate-x-1/2 bg-gray-900 text-white text-[10px] px-2 py-1 rounded whitespace-nowrap z-10">
											Budget Utilization <span class="text-green-400 ml-1">78%</span>
										</div>
										<div class="absolute bottom-full mb-1 left-1/2 -translate-x-1/2 w-0 h-0 border-l-[4px] border-l-transparent border-r-[4px] border-r-transparent border-t-[4px] border-t-gray-900"></div>
									</div>
									<!-- March -->
									<div class="w-8 flex flex-col gap-0.5 items-center relative">
										<div class="w-full h-14 rounded-t-sm" style="background: oklch(0.696 0.17 162.48)"></div>
										<div class="w-full h-20" style="background: oklch(0.596 0.145 163.225)"></div>
										<div class="w-full h-32" style="background: oklch(0.508 0.118 165.612)"></div>
										<div class="absolute -bottom-6 text-[10px] text-gray-500">Mar</div>
									</div>
								</div>
							</div>
						</div>

						<!-- Chart 2: Donut -->
						<div class="col-span-2 bg-white rounded-lg border border-gray-200 p-4 shadow-sm">
							<div class="flex items-center justify-between mb-4">
								<h3 class="text-sm font-medium text-gray-900">Approvals by status</h3>
								<MoreHorizontal size={14} class="text-gray-400" />
							</div>
							<div class="flex flex-wrap gap-2 text-[10px] text-gray-500 mb-8">
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full bg-green-500"></div> Approved</div>
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full bg-yellow-500"></div> Pending</div>
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full bg-blue-500"></div> In Review</div>
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full bg-red-400"></div> Rejected</div>
							</div>

							<!-- Mock Donut Chart -->
							<div class="relative w-48 h-48 mx-auto">
								<svg viewBox="0 0 100 100" class="w-full h-full transform -rotate-90">
									<circle cx="50" cy="50" r="40" fill="transparent" stroke="#dcfce7" stroke-width="16" /> <!-- Base -->
									<circle cx="50" cy="50" r="40" fill="transparent" stroke="#22c55e" stroke-width="16" stroke-dasharray="120 251" stroke-dashoffset="0" /> <!-- Green segment -->
									<circle cx="50" cy="50" r="40" fill="transparent" stroke="#eab308" stroke-width="16" stroke-dasharray="60 251" stroke-dashoffset="-120" /> <!-- Yellow segment -->
									<circle cx="50" cy="50" r="40" fill="transparent" stroke="#3b82f6" stroke-width="16" stroke-dasharray="50 251" stroke-dashoffset="-180" /> <!-- Blue segment -->
									<circle cx="50" cy="50" r="40" fill="transparent" stroke="#f87171" stroke-width="16" stroke-dasharray="21 251" stroke-dashoffset="-230" /> <!-- Red segment -->
								</svg>
								<div class="absolute inset-0 flex items-center justify-center flex-col">
									<span class="text-2xl font-bold text-gray-900">342</span>
									<span class="text-xs text-gray-500">Total</span>
								</div>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>

	<!-- Logos -->
	<div class="mt-20 flex flex-wrap justify-center items-center gap-12 opacity-60">
		<div class="text-gray-500 text-sm font-medium">Trusted by leading German SMEs:</div>
		<div class="font-bold text-lg text-gray-700">Bosch</div>
		<div class="font-bold text-lg text-gray-700">Siemens</div>
		<div class="font-bold text-lg text-gray-700">METRO</div>
		<div class="font-bold text-lg text-gray-700">Würth</div>
		<div class="font-bold text-lg text-gray-700">Knauf</div>
		<div class="text-gray-500 text-sm">+ 10,000 more</div>
	</div>
</section>
