<script lang="ts">
	import { onMount } from 'svelte';

	let mounted = false;

	onMount(() => {
		mounted = true;
	});


    let demoData = true;

    function getTotalActivePlayers() {
        if (demoData) { return 12345; }
        // Await Zffu's implementation of a webhook to track actual
        // data, then call that API here to add to the site.
    }

    function getTotalActiveRealms() {
        if (demoData) { return 12; }
        // Await Zffu's implementation of a webhook to track actual
        // data, then call that API here to add to the site.
    }

</script>

<svelte:head>
	<title>Cavernfall - Epic MMORPG Adventure</title>
	<meta name="description" content="Embark on an epic journey in Cavernfall, a thrilling MMORPG where heroes forge their destiny through ancient realms filled with magic, monsters, and legendary treasures." />
</svelte:head>

<!-- Background -->
<div class="fixed inset-0 -z-10 overflow-hidden">
	<!-- Gradient Background -->
	<div class="absolute inset-0 bg-gradient-to-br from-purple-900 via-blue-900 to-indigo-900"></div>
	
	<!-- Animated Background Shapes -->
	<div class="absolute top-1/4 left-1/4 w-96 h-96 bg-purple-500 rounded-full mix-blend-multiply filter blur-xl opacity-20 animate-pulse"></div>
	<div class="absolute top-1/3 right-1/4 w-96 h-96 bg-cyan-500 rounded-full mix-blend-multiply filter blur-xl opacity-20 animate-pulse animation-delay-2000"></div>
	<div class="absolute bottom-1/4 left-1/3 w-96 h-96 bg-pink-500 rounded-full mix-blend-multiply filter blur-xl opacity-20 animate-pulse animation-delay-4000"></div>
</div>

<!-- Main Content -->
<main class="min-h-screen">
	<!-- Hero Section -->
	<section class="relative px-6 pt-20 pb-32">
		<div class="max-w-7xl mx-auto">
			<!-- Glass Container -->
			<div class="backdrop-blur-md bg-white/10 border border-white/20 rounded-3xl p-8 md:p-12 shadow-2xl">
				<div class="text-center">
					<!-- Logo/Brand -->
					<div class="inline-flex items-center justify-center w-20 h-20 bg-gradient-to-r from-purple-500 to-cyan-500 rounded-2xl mb-8 shadow-lg">
						<svg class="w-10 h-10 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
							<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 3l1.664 1.664M21 21l-1.664-1.664m-8.485 0L7.536 16.02a2 2 0 01-2.828-2.828l3.314-3.314m8.485 8.485l3.314-3.314a2 2 0 00-2.828-2.828L13.68 9.15m0 0L9.734 5.204a2 2 0 10-2.828 2.828L10.852 12.18"></path>
						</svg>
					</div>
					
					<!-- Hero Text -->
					<h1 class="text-5xl md:text-7xl font-bold text-white mb-6">
						Welcome to
                        <span class="bg-gradient-to-r from-purple-400 to-cyan-400 bg-clip-text text-transparent drop-shadow-lg">
                            Cavernfall
                        </span>
					</h1>
					
					<p class="text-xl md:text-2xl text-gray-200 mb-12 max-w-3xl mx-auto leading-relaxed">
						Forge your story in the legendary realms of Cavernfall. Unite with heroes across the world, conquer ancient dungeons, and master powerful magic in the ultimate MMORPG adventure.
					</p>
					
					<!-- CTA Buttons -->
					<div class="flex flex-col sm:flex-row gap-4 justify-center items-center">
						<button class="backdrop-blur-md bg-white/20 hover:bg-white/30 border border-white/30 text-white px-8 py-4 rounded-2xl font-semibold transition-all duration-300 hover:scale-105 shadow-lg">
                            <svg class="w-6 h-6 inline-block mr-2 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 16v2a2 2 0 002 2h12a2 2 0 002-2v-2M7 10l5 5m0 0l5-5m-5 5V4"/>
                            </svg>
                            Download Now
						</button>
                        <button class="backdrop-blur-md bg-gradient-to-r from-[#5865F2]/20 to-[#23272A]/20 hover:from-[#5865F2]/30 hover:to-[#23272A]/30 border border-[#5865F2]/30 text-white px-8 py-4 rounded-2xl font-semibold transition-all duration-300 hover:scale-105 shadow-lg flex items-center gap-2">
                            <svg class="w-6 h-6 text-[#5865F2]" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M20.317 4.369a19.791 19.791 0 00-4.885-1.515.074.074 0 00-.079.037c-.211.375-.447.864-.614 1.249a18.233 18.233 0 00-5.487 0 12.522 12.522 0 00-.625-1.249.077.077 0 00-.078-.037A19.736 19.736 0 003.683 4.369a.069.069 0 00-.032.027C.533 8.725-.32 13.01.099 17.251a.082.082 0 00.031.057c2.052 1.507 4.042 2.422 5.993 3.029a.077.077 0 00.084-.027c.462-.635.873-1.304 1.226-2.005a.076.076 0 00-.041-.104c-.652-.247-1.272-.549-1.872-.892a.077.077 0 01-.008-.127c.126-.094.252-.192.372-.291a.075.075 0 01.077-.01c3.927 1.793 8.18 1.793 12.061 0a.075.075 0 01.078.009c.12.099.246.197.372.291a.077.077 0 01-.007.127 12.298 12.298 0 01-1.873.892.076.076 0 00-.04.105c.36.7.771 1.369 1.225 2.004a.076.076 0 00.084.028c1.961-.607 3.951-1.522 5.993-3.029a.077.077 0 00.031-.057c.5-5.177-.838-9.418-3.549-12.855a.061.061 0 00-.031-.028zM8.02 15.331c-1.183 0-2.156-1.085-2.156-2.419 0-1.334.955-2.419 2.157-2.419 1.21 0 2.174 1.094 2.156 2.419 0 1.334-.955 2.419-2.157 2.419zm7.974 0c-1.183 0-2.156-1.085-2.156-2.419 0-1.334.955-2.419 2.156-2.419 1.21 0 2.174 1.094 2.156 2.419 0 1.334-.946 2.419-2.156 2.419z"/>
                            </svg>
                            Join the Discord!
                        </button>
					</div>
				</div>
			</div>
		</div>
	</section>

	<!-- Features Section -->
	<section class="px-6 pb-20">
		<div class="max-w-7xl mx-auto">
			<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
				<!-- Feature Card 1 -->
				<div class="backdrop-blur-md bg-white/5 border border-white/10 rounded-2xl p-6 hover:bg-white/10 transition-all duration-300 hover:scale-105 shadow-xl group">
					<div class="w-12 h-12 bg-gradient-to-r from-purple-500 to-pink-500 rounded-xl flex items-center justify-center mb-4 group-hover:scale-110 transition-transform duration-300">
						<svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
							<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path>
						</svg>
					</div>
					<h3 class="text-xl font-semibold text-white mb-3">⚡ Dynamic Combat</h3>
					<p class="text-gray-300 leading-relaxed">Experience lightning-fast, skill-based combat with devastating spells and legendary weapons.</p>
				</div>

				<!-- Feature Card 2 -->
				<div class="backdrop-blur-md bg-white/5 border border-white/10 rounded-2xl p-6 hover:bg-white/10 transition-all duration-300 hover:scale-105 shadow-xl group">
					<div class="w-12 h-12 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-xl flex items-center justify-center mb-4 group-hover:scale-110 transition-transform duration-300">
						<svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
							<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 4.354a4 4 0 110 5.292M15 21H3v-1a6 6 0 0112 0v1zm0 0h6v-1a6 6 0 00-9-5.197m13.5-9a2.5 2.5 0 11-5 0 2.5 2.5 0 015 0z"></path>
						</svg>
					</div>
					<h3 class="text-xl font-semibold text-white mb-3">🌍 Massive Multiplayer</h3>
					<p class="text-gray-300 leading-relaxed">Join {getTotalActivePlayers()} other player(s) in epic raids, guild wars, and collaborative questing adventures.</p>
				</div>

				<!-- Feature Card 3 -->
				<div class="backdrop-blur-md bg-white/5 border border-white/10 rounded-2xl p-6 hover:bg-white/10 transition-all duration-300 hover:scale-105 shadow-xl group">
					<div class="w-12 h-12 bg-gradient-to-r from-pink-500 to-purple-500 rounded-xl flex items-center justify-center mb-4 group-hover:scale-110 transition-transform duration-300">
						<svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
							<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M11.049 2.927c.3-.921 1.603-.921 1.902 0l1.519 4.674a1 1 0 00.95.69h4.915c.969 0 1.371 1.24.588 1.81l-3.976 2.888a1 1 0 00-.363 1.118l1.518 4.674c.3.922-.755 1.688-1.538 1.118l-3.976-2.888a1 1 0 00-1.176 0l-3.976 2.888c-.783.57-1.838-.197-1.538-1.118l1.518-4.674a1 1 0 00-.363-1.118l-3.976-2.888c-.784-.57-.38-1.81.588-1.81h4.914a1 1 0 00.951-.69l1.519-4.674z"></path>
						</svg>
					</div>
					<h3 class="text-xl font-semibold text-white mb-3">🏆 Epic Progression</h3>
					<p class="text-gray-300 leading-relaxed">Unlock legendary skills, craft mythical gear, and ascend through ranks to become a true champion.</p>
				</div>
			</div>
		</div>
	</section>

	<!-- Stats Section -->
	<section class="px-6 pb-20">
		<div class="max-w-5xl mx-auto">
			<div class="backdrop-blur-md bg-white/5 border border-white/10 rounded-3xl p-8 md:p-12 shadow-xl">
				<div class="grid grid-cols-2 md:grid-cols-4 gap-8">
					<div class="text-center">
						<div class="text-3xl md:text-4xl font-bold text-white mb-2">{getTotalActivePlayers()}+</div>
						<div class="text-gray-300 text-sm md:text-base">Active Heroes</div>
					</div>
					<div class="text-center">
						<div class="text-3xl md:text-4xl font-bold text-white mb-2">{getTotalActiveRealms()}</div>
						<div class="text-gray-300 text-sm md:text-base">Epic Realms</div>
					</div>
					<div class="text-center">
						<div class="text-3xl md:text-4xl font-bold text-white mb-2">200+</div>
						<div class="text-gray-300 text-sm md:text-base">Legendary Quests</div>
					</div>
					<div class="text-center">
						<div class="text-3xl md:text-4xl font-bold text-white mb-2">∞</div>
						<div class="text-gray-300 text-sm md:text-base">Adventures</div>
					</div>
				</div>
			</div>
		</div>
	</section>
</main>

<style>
	/* Custom animations are now in global CSS */
	
	/* Smooth scrolling - applied globally */
	:global(html) {
		scroll-behavior: smooth;
	}
	
	/* Enhanced glassmorphism */
	.backdrop-blur-md {
		backdrop-filter: blur(16px);
		-webkit-backdrop-filter: blur(16px);
	}
</style>