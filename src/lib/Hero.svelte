<script lang="ts">
	import { ArrowRight, Sparkles, Check, Clock, Paperclip, Send, Bot, User, CheckCircle2 } from 'lucide-svelte';
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

	<!-- AI Chat Flow Preview -->
	<div class="relative rounded-xl overflow-hidden border border-gray-200 bg-gradient-to-b from-gray-50 to-white text-left mx-auto max-w-[1200px]">
		<!-- Chat Interface Container -->
		<div class="flex flex-col h-[650px] bg-white p-8">
			<!-- Welcome Header -->
			<div class="text-center mb-8">
				<h2 class="text-3xl font-semibold text-gray-900 mb-2">Hi Stefan, how can I help you today?</h2>
				<p class="text-sm text-gray-500">Simply describe what you need and I'll handle the rest</p>
			</div>

			<!-- Chat Messages -->
			<div class="flex-1 space-y-4 mb-6 overflow-y-auto">
				<!-- User Message -->
				<div class="flex justify-end">
					<div class="flex items-start gap-3 max-w-[70%]">
						<div class="bg-black text-white rounded-2xl rounded-tr-sm px-4 py-3">
							<p class="text-sm">I need 5 new MacBook Pros for the development team</p>
						</div>
						<div class="w-8 h-8 rounded-full bg-blue-100 flex items-center justify-center flex-shrink-0">
							<User size={16} class="text-blue-600" />
						</div>
					</div>
				</div>

				<!-- AI Response -->
				<div class="flex justify-start">
					<div class="flex items-start gap-3 max-w-[70%]">
						<div class="w-8 h-8 rounded-full bg-gradient-to-br from-purple-500 to-blue-500 flex items-center justify-center flex-shrink-0">
							<Bot size={16} class="text-white" />
						</div>
						<div class="bg-gray-100 rounded-2xl rounded-tl-sm px-4 py-3">
							<p class="text-sm text-gray-900 mb-3">I found the perfect match for your team. I've created a purchase request with the best available pricing.</p>
							<div class="flex items-center gap-2 text-xs text-gray-600">
								<Sparkles size={12} class="text-purple-500" />
								<span>Automatically routed to Bettina for approval</span>
							</div>
						</div>
					</div>
				</div>

				<!-- AI Processing Indicator -->
				<div class="flex justify-start">
					<div class="flex items-start gap-3 max-w-[70%]">
						<div class="w-8 h-8 rounded-full bg-gradient-to-br from-purple-500 to-blue-500 flex items-center justify-center flex-shrink-0">
							<Bot size={16} class="text-white" />
						</div>
						<div class="bg-gray-100 rounded-2xl rounded-tl-sm px-4 py-3">
							<div class="flex items-center gap-2 text-sm text-gray-600">
								<div class="flex gap-1">
									<div class="w-2 h-2 bg-purple-500 rounded-full animate-bounce" style="animation-delay: 0ms"></div>
									<div class="w-2 h-2 bg-purple-500 rounded-full animate-bounce" style="animation-delay: 150ms"></div>
									<div class="w-2 h-2 bg-purple-500 rounded-full animate-bounce" style="animation-delay: 300ms"></div>
								</div>
								<span>Processing approval workflow</span>
							</div>
						</div>
					</div>
				</div>
			</div>

			<!-- Purchase Request Cards -->
			<div class="border-t border-gray-200 pt-6">
				<div class="flex items-center gap-2 mb-4">
					<h3 class="text-sm font-medium text-gray-900">Active requests</h3>
					<span class="text-xs text-gray-500">3 items</span>
				</div>
				
				<div class="flex gap-4 overflow-x-auto pb-2">
					<!-- Card 1: Approved -->
					<div class="flex-shrink-0 w-[280px] bg-white border border-gray-200 rounded-lg p-4">
						<div class="flex items-center justify-between mb-3">
							<span class="inline-flex items-center gap-1 text-xs font-medium text-green-700 bg-green-50 px-2 py-1 rounded-full">
								<CheckCircle2 size={12} />
								Approved
							</span>
							<span class="text-xs text-gray-500">002968</span>
						</div>
						<h4 class="text-sm font-medium text-gray-900 mb-1">Nordvlies Office Chairs</h4>
						<p class="text-xs text-gray-500 mb-3">Price (net) €395.73</p>
						<div class="space-y-2">
							<div class="flex items-center gap-2 text-xs text-gray-600">
								<Check size={12} class="text-green-500" />
								<span>Approved by Stefan</span>
							</div>
							<div class="flex items-center gap-2 text-xs text-gray-600">
								<Clock size={12} class="text-blue-500" />
								<span>Products are on its way</span>
							</div>
						</div>
					</div>

					<!-- Card 2: Pending -->
					<div class="flex-shrink-0 w-[280px] bg-white border border-gray-200 rounded-lg p-4">
						<div class="flex items-center justify-between mb-3">
							<span class="inline-flex items-center gap-1 text-xs font-medium text-yellow-700 bg-yellow-50 px-2 py-1 rounded-full">
								<Clock size={12} />
								Pending
							</span>
							<span class="text-xs text-gray-500">002866</span>
						</div>
						<h4 class="text-sm font-medium text-gray-900 mb-1">MacBook Pro</h4>
						<p class="text-xs text-gray-500 mb-3">5 units • €12,495.00</p>
						<div class="space-y-2">
							<div class="flex items-center gap-2 text-xs text-gray-600">
								<Clock size={12} class="text-yellow-500" />
								<span>Pending approval from Bettina</span>
							</div>
							<div class="flex items-center gap-2 text-xs text-gray-600">
								<Sparkles size={12} class="text-purple-500" />
								<span>Auto-matched best vendor</span>
							</div>
						</div>
					</div>

					<!-- Card 3: Pending -->
					<div class="flex-shrink-0 w-[280px] bg-white border border-gray-200 rounded-lg p-4">
						<div class="flex items-center justify-between mb-3">
							<span class="inline-flex items-center gap-1 text-xs font-medium text-yellow-700 bg-yellow-50 px-2 py-1 rounded-full">
								<Clock size={12} />
								Pending
							</span>
							<span class="text-xs text-gray-500">002865</span>
						</div>
						<h4 class="text-sm font-medium text-gray-900 mb-1">Logitech Headset</h4>
						<p class="text-xs text-gray-500 mb-3">Price (net) €89.99</p>
						<div class="space-y-2">
							<div class="flex items-center gap-2 text-xs text-gray-600">
								<Clock size={12} class="text-yellow-500" />
								<span>Pending approval from Bettina</span>
							</div>
						</div>
					</div>
				</div>
			</div>

			<!-- Chat Input -->
			<div class="mt-6 relative">
				<div class="flex items-center gap-3 bg-gray-50 border border-gray-200 rounded-xl px-4 py-3">
					<button class="text-gray-400 hover:text-gray-600 transition-colors">
						<Paperclip size={18} />
					</button>
					<input 
						type="text" 
						placeholder="Tell me what you need" 
						class="flex-1 bg-transparent text-sm text-gray-900 placeholder-gray-400 outline-none"
					/>
					<button class="bg-black text-white p-2 rounded-lg hover:bg-gray-800 transition-colors">
						<Send size={16} />
					</button>
				</div>
				<p class="text-xs text-gray-400 mt-2 text-center">Upload files for comparison, automated request creation and much more</p>
			</div>
		</div>
	</div>

	<!-- Integration Section -->
	<div class="mt-20 text-center max-w-3xl mx-auto">
		<p class="text-sm font-medium text-gray-500 mb-4">Built to fit into what you already use. Plug in. Don't rebuild.</p>
		<p class="text-base text-gray-700 leading-relaxed">
			Hivebuy integrates seamlessly with your existing tools and workflows—no complex setup, no disruption. Connect to any ERP system, embed Hivebuy into your current stack, and deploy the Hivebuy chat agent directly in tools like Microsoft Teams. Get value from day one with an implementation that's as effortless as it is powerful.
		</p>
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
