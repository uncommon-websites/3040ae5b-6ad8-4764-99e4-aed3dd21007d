<script lang="ts">
	import { ArrowRight, Zap, Bot, Database, BarChart3, Mail, MessageSquare, Calendar, CheckCircle2, Search, Plus, MoreHorizontal } from 'lucide-svelte';
</script>

<section class="max-w-[1200px] mx-auto px-6 py-20">
	<div class="mb-20 max-w-2xl">
		<h2 class="text-4xl font-serif text-gray-900 mb-6">
			Procurement at full control. <span class="text-gray-500 font-sans text-xl font-normal block mt-4">Execute your procurement strategy with precision. Design automated approval workflows, track budgets in real-time, integrate with your ERP and build detailed spending reports — all in one platform.</span>
		</h2>
	</div>

	<div class="border border-gray-200 rounded-xl overflow-hidden bg-white shadow-sm">
		<!-- Row 1: Automated approval workflows -->
		<div class="grid grid-cols-1 md:grid-cols-3 border-b border-gray-200">
			<div class="p-12 flex flex-col justify-between border-r border-gray-200">
				<div>
					<h3 class="text-xl font-bold text-gray-900 mb-4">Automated approval workflows</h3>
					<p class="text-gray-500 leading-relaxed mb-8">
						You're in control. Automate even the most complex approval processes with configurable workflows that route requests to the right approvers instantly.
					</p>
				</div>
				<a href="#" class="inline-flex items-center gap-2 text-sm font-medium text-gray-900 hover:opacity-70 transition-opacity">
					Explore workflows <ArrowRight size={16} />
				</a>
			</div>
			<div class="col-span-2 bg-gray-50/50 p-12 flex items-center justify-center overflow-hidden relative">
				<!-- Workflow Diagram Mockup -->
				<div class="relative w-full max-w-lg">
					<!-- Trigger -->
					<div class="absolute top-0 left-0 bg-white border border-gray-200 rounded-lg p-3 shadow-sm w-64 z-10">
						<div class="flex items-center gap-2 text-xs font-medium text-gray-500 mb-2">
							<Zap size={12} /> Trigger
						</div>
						<div class="text-sm font-medium text-gray-900">When Purchase Order created</div>
						<div class="text-xs text-gray-400 mt-1">Trigger when new PO exceeds €5,000</div>
					</div>

					<!-- Path -->
					<svg class="absolute top-16 left-32 w-full h-40 pointer-events-none" style="z-index: 0;">
						<path d="M 0 0 V 20 H 100 V 40" fill="none" stroke="#e5e7eb" stroke-width="2" />
						<path d="M 0 0 V 20 H -100 V 40" fill="none" stroke="#e5e7eb" stroke-width="2" />
					</svg>

					<!-- Branch 1 -->
					<div class="absolute top-32 -left-20 bg-white border border-gray-200 rounded-lg p-3 shadow-sm w-56">
						<div class="flex items-center gap-2 text-xs font-medium text-gray-500 mb-2">
							<div class="w-2 h-2 rounded-full" style="background: oklch(0.696 0.17 162.48)"></div> Route
						</div>
						<div class="text-sm font-medium text-gray-900">Budget check</div>
						<div class="mt-2 flex gap-2">
							<span class="px-2 py-0.5 bg-green-100 text-green-700 text-[10px] rounded">Available</span>
							<span class="px-2 py-0.5 bg-red-100 text-red-700 text-[10px] rounded">Exceeded</span>
						</div>
					</div>

					<!-- Branch 2 -->
					<div class="absolute top-32 left-40 bg-white border border-gray-200 rounded-lg p-3 shadow-sm w-56">
						<div class="flex items-center gap-2 text-xs font-medium text-gray-500 mb-2">
							<Mail size={12} /> Notify
						</div>
						<div class="text-sm font-medium text-gray-900">Send to approver</div>
						<div class="flex items-center gap-2 mt-2">
							<div class="w-6 h-6 rounded-full bg-gray-100 flex items-center justify-center text-[10px]">BF</div>
							<span class="text-xs text-gray-500">Bettina Fischer</span>
						</div>
					</div>
				</div>
				
				<!-- Decorative geometric shape -->
				<div class="absolute bottom-10 right-10 opacity-20">
					<svg width="100" height="100" viewBox="0 0 100 100" fill="none">
						<path d="M50 0L93.3013 25V75L50 100L6.69873 75V25L50 0Z" stroke="black" stroke-width="1"/>
						<path d="M50 0V50M93.3013 25L50 50M93.3013 75L50 50M50 100V50M6.69873 75L50 50M6.69873 25L50 50" stroke="black" stroke-width="1"/>
					</svg>
				</div>
			</div>
		</div>

		<!-- Row 2: Real-time budget tracking -->
		<div class="grid grid-cols-1 md:grid-cols-3 border-b border-gray-200">
			<div class="p-12 flex flex-col justify-between border-r border-gray-200">
				<div>
					<h3 class="text-xl font-bold text-gray-900 mb-4">Real-time budget tracking</h3>
					<p class="text-gray-500 leading-relaxed mb-8">
						Monitor spending across departments, categories, and vendors in real-time. Get instant alerts when budgets are at risk and make informed decisions faster.
					</p>
				</div>
				<a href="#" class="inline-flex items-center gap-2 text-sm font-medium text-gray-900 hover:opacity-70 transition-opacity">
					Explore budgets <ArrowRight size={16} />
				</a>
			</div>
			<div class="col-span-2 bg-gray-50/50 p-12 flex items-center justify-center relative">
				<div class="bg-white rounded-xl shadow-sm border border-gray-200 w-full max-w-md overflow-hidden">
					<div class="p-3 border-b border-gray-100 flex items-center gap-2 bg-gray-50/50">
						<BarChart3 size={16} style="color: oklch(0.696 0.17 162.48)" />
						<span class="text-xs font-medium text-gray-700">Budget Alert</span>
					</div>
					<div class="p-4 space-y-4">
						<div class="flex gap-3">
							<div class="w-8 h-8 rounded-full flex items-center justify-center flex-shrink-0" style="background: oklch(0.95 0.052 163.051)">
								<BarChart3 size={16} style="color: oklch(0.696 0.17 162.48)" />
							</div>
							<div class="flex-1">
								<div class="bg-yellow-50 border border-yellow-200 rounded-lg p-3 text-sm text-gray-800 mb-2">
									<p class="font-medium mb-1">Marketing Budget at 85%</p>
									<p class="text-gray-600 text-xs">Q1 Marketing budget has reached €42,500 of €50,000</p>
								</div>
								
								<div class="bg-white border border-gray-200 rounded-lg p-3 text-sm text-gray-800 mb-2 shadow-sm">
									<div class="flex items-center justify-between mb-2">
										<span class="font-medium text-xs text-gray-500">Department Breakdown</span>
									</div>
									<div class="space-y-2">
										<div class="flex items-center justify-between text-xs">
											<span>Digital Ads</span>
											<span class="font-medium">€28,000</span>
										</div>
										<div class="flex items-center justify-between text-xs">
											<span>Events</span>
											<span class="font-medium">€9,500</span>
										</div>
										<div class="flex items-center justify-between text-xs">
											<span>Content</span>
											<span class="font-medium">€5,000</span>
										</div>
									</div>
								</div>

								<div class="bg-white border border-gray-200 rounded-lg p-3 text-sm text-gray-800 shadow-sm">
									<div class="flex items-center gap-2 mb-2">
										<div class="w-4 h-4 rounded flex items-center justify-center text-[10px]" style="background: oklch(0.696 0.17 162.48); color: white">!</div>
										<span class="font-medium">Remaining: €7,500</span>
									</div>
									<p class="text-gray-500 text-xs">Projected to exceed by €3,200 if current trend continues</p>
								</div>
							</div>
						</div>
					</div>
				</div>
				
				<!-- Decorative geometric shape -->
				<div class="absolute bottom-10 right-10 opacity-20">
					<svg width="100" height="100" viewBox="0 0 100 100" fill="none">
						<circle cx="50" cy="50" r="40" stroke="black" stroke-width="1"/>
						<path d="M50 10 C 70 30, 70 70, 50 90 C 30 70, 30 30, 50 10" stroke="black" stroke-width="1" fill="none"/>
						<path d="M10 50 C 30 30, 70 30, 90 50 C 70 70, 30 70, 10 50" stroke="black" stroke-width="1" fill="none"/>
					</svg>
				</div>
			</div>
		</div>

		<!-- Row 3: ERP Integration -->
		<div class="grid grid-cols-1 md:grid-cols-3 border-b border-gray-200">
			<div class="p-12 flex flex-col justify-between border-r border-gray-200">
				<div>
					<h3 class="text-xl font-bold text-gray-900 mb-4">Seamless ERP integration</h3>
					<p class="text-gray-500 leading-relaxed mb-8">
						Pre-configured connectors for SAP, DATEV, and other leading ERP systems. Sync purchase orders, invoices, and vendor data automatically.
					</p>
				</div>
				<a href="#" class="inline-flex items-center gap-2 text-sm font-medium text-gray-900 hover:opacity-70 transition-opacity">
					Explore integrations <ArrowRight size={16} />
				</a>
			</div>
			<div class="col-span-2 bg-gray-50/50 p-12 flex items-center justify-center relative">
				<div class="relative w-full max-w-md h-64 flex items-center justify-center">
					<!-- Center Logo -->
					<div class="w-16 h-16 bg-black rounded-xl flex items-center justify-center z-10 shadow-lg">
						<svg width="32" height="32" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
							<path d="M12 4L4 8V16L12 20L20 16V8L12 4Z" fill="oklch(0.696 0.17 162.48)"/>
							<path d="M12 4V12M4 8L12 12M20 8L12 12M12 20V12M4 16L12 12M20 16L12 12" stroke="white" stroke-width="1"/>
						</svg>
					</div>

					<!-- Connecting Lines -->
					<svg class="absolute inset-0 w-full h-full pointer-events-none">
						<line x1="50%" y1="50%" x2="20%" y2="20%" stroke="#e5e7eb" stroke-width="1" />
						<line x1="50%" y1="50%" x2="80%" y2="20%" stroke="#e5e7eb" stroke-width="1" />
						<line x1="50%" y1="50%" x2="20%" y2="80%" stroke="#e5e7eb" stroke-width="1" />
						<line x1="50%" y1="50%" x2="80%" y2="80%" stroke="#e5e7eb" stroke-width="1" />
						<line x1="50%" y1="50%" x2="50%" y2="15%" stroke="#e5e7eb" stroke-width="1" />
						<line x1="50%" y1="50%" x2="50%" y2="85%" stroke="#e5e7eb" stroke-width="1" />
					</svg>

					<!-- ERP System Icons -->
					<div class="absolute top-10 left-20 bg-white p-3 rounded-lg shadow-sm border border-gray-100">
						<div class="text-xs font-bold text-gray-700">SAP</div>
					</div>
					<div class="absolute top-10 right-20 bg-white p-3 rounded-lg shadow-sm border border-gray-100">
						<div class="text-xs font-bold text-gray-700">DATEV</div>
					</div>
					<div class="absolute bottom-10 left-20 bg-white p-3 rounded-lg shadow-sm border border-gray-100">
						<div class="text-xs font-bold text-gray-700">Lexware</div>
					</div>
					<div class="absolute bottom-10 right-20 bg-white p-3 rounded-lg shadow-sm border border-gray-100">
						<div class="text-xs font-bold text-gray-700">SAGE</div>
					</div>
					<div class="absolute top-4 left-1/2 -translate-x-1/2 bg-white p-3 rounded-lg shadow-sm border border-gray-100">
						<div class="text-xs font-bold text-gray-700">Oracle</div>
					</div>
					<div class="absolute bottom-4 left-1/2 -translate-x-1/2 bg-white p-3 rounded-lg shadow-sm border border-gray-100">
						<div class="text-xs font-bold text-gray-700">Navision</div>
					</div>
				</div>
				
				<!-- Decorative geometric shape -->
				<div class="absolute bottom-10 right-10 opacity-20">
					<svg width="100" height="100" viewBox="0 0 100 100" fill="none">
						<rect x="25" y="25" width="50" height="50" stroke="black" stroke-width="1" transform="rotate(45 50 50)"/>
						<rect x="25" y="25" width="50" height="50" stroke="black" stroke-width="1"/>
					</svg>
				</div>
			</div>
		</div>

		<!-- Row 4: Spend analytics -->
		<div class="grid grid-cols-1 md:grid-cols-3">
			<div class="p-12 flex flex-col justify-between border-r border-gray-200">
				<div>
					<h3 class="text-xl font-bold text-gray-900 mb-4">Spend analytics</h3>
					<p class="text-gray-500 leading-relaxed mb-8">
						Create real-time spending reports that scale with your data. Visualize procurement patterns, identify savings opportunities, and get deep insights in seconds.
					</p>
				</div>
				<a href="#" class="inline-flex items-center gap-2 text-sm font-medium text-gray-900 hover:opacity-70 transition-opacity">
					Explore analytics <ArrowRight size={16} />
				</a>
			</div>
			<div class="col-span-2 bg-gray-50/50 p-12 flex items-center justify-center relative">
				<div class="grid grid-cols-2 gap-6 w-full max-w-lg">
					<!-- Chart 1 -->
					<div class="bg-white p-4 rounded-xl border border-gray-200 shadow-sm">
						<div class="flex items-center justify-between mb-4">
							<div class="text-xs font-medium text-gray-500">Weekly Spend</div>
							<MoreHorizontal size={14} class="text-gray-400" />
						</div>
						<div class="h-32 flex items-end gap-2 justify-between px-2">
							<div class="w-full h-[40%] rounded-t-sm" style="background: oklch(0.845 0.143 164.978)"></div>
							<div class="w-full h-[60%] rounded-t-sm" style="background: oklch(0.765 0.177 163.223)"></div>
							<div class="w-full h-[30%] rounded-t-sm" style="background: oklch(0.696 0.17 162.48)"></div>
							<div class="w-full h-[80%] rounded-t-sm" style="background: oklch(0.596 0.145 163.225)"></div>
							<div class="w-full h-[50%] rounded-t-sm" style="background: oklch(0.508 0.118 165.612)"></div>
						</div>
						<div class="flex justify-between mt-2 text-[10px] text-gray-400">
							<span>Mon</span>
							<span>Tue</span>
							<span>Wed</span>
							<span>Thu</span>
							<span>Fri</span>
						</div>
					</div>

					<!-- List -->
					<div class="bg-white p-4 rounded-xl border border-gray-200 shadow-sm space-y-3">
						<div class="flex items-center justify-between mb-2">
							<div class="text-xs font-medium text-gray-500">Top Vendors</div>
						</div>
						<div class="flex items-center gap-2 text-xs">
							<div class="w-2 h-2 rounded-full bg-green-500"></div>
							<span class="flex-1">Siemens AG</span>
							<span class="font-medium">€52k</span>
						</div>
						<div class="flex items-center gap-2 text-xs">
							<div class="w-2 h-2 rounded-full bg-blue-500"></div>
							<span class="flex-1">METRO AG</span>
							<span class="font-medium">€38k</span>
						</div>
						<div class="flex items-center gap-2 text-xs">
							<div class="w-2 h-2 rounded-full bg-purple-500"></div>
							<span class="flex-1">Würth Group</span>
							<span class="font-medium">€45k</span>
						</div>
						<div class="flex items-center gap-2 text-xs">
							<div class="w-2 h-2 rounded-full bg-orange-500"></div>
							<span class="flex-1">Bosch GmbH</span>
							<span class="font-medium">€62k</span>
						</div>
					</div>
				</div>
				
				<!-- Decorative geometric shape -->
				<div class="absolute bottom-10 right-10 opacity-20">
					<svg width="100" height="100" viewBox="0 0 100 100" fill="none">
						<path d="M20 80 L 50 30 L 80 80 Z" stroke="black" stroke-width="1"/>
						<path d="M20 80 L 20 50 L 50 30" stroke="black" stroke-width="1"/>
						<path d="M80 80 L 80 50 L 50 30" stroke="black" stroke-width="1"/>
					</svg>
				</div>
			</div>
		</div>
	</div>
</section>
