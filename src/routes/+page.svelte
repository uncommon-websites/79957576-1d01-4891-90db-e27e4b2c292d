<script lang="ts">
	import { onMount } from 'svelte';

	let scrollY = 0;
</script>

<svelte:window bind:scrollY />

<div class="font-sans text-gray-900 antialiased selection:bg-orange-200 selection:text-orange-900">
	<!-- Navigation / Header (Implicit in design, maybe just the logo or minimal) -->
	<!-- The screenshot doesn't explicitly show a header bar, but usually there is one. 
         I will assume a minimal or transparent one, or just the content. 
         The "W." ribbon is fixed on the right. -->
    
    <div class="fixed top-0 right-0 z-50 h-full pointer-events-none">
        <div class="absolute top-[15vh] right-0 bg-black text-white w-8 md:w-10 py-4 flex flex-col items-center justify-center font-bold text-xs pointer-events-auto cursor-pointer hover:bg-gray-900 transition-colors">
            <span class="writing-vertical-rl rotate-180 transform">Site of the Day</span>
            <span class="mt-2 font-serif text-lg">W.</span>
        </div>
    </div>

	<!-- Hero Section -->
	<section class="relative min-h-screen w-full bg-gradient-to-b from-[#1a2c4e] via-[#4a6b9c] to-[#fdfbf7] text-white px-6 md:px-12 lg:px-24 pt-32 pb-24 flex flex-col justify-between">
		<div class="max-w-5xl">
			<h1 class="font-serif text-5xl md:text-7xl lg:text-8xl leading-[1.1] md:leading-[1.1] tracking-tight">
				New Genre is a global design & technology studio accelerating tomorrow's ideas.
			</h1>
		</div>

		<div class="mt-24">
			<a href="#work" class="inline-flex items-center justify-center px-6 py-3 border border-white/30 rounded-full text-sm font-medium hover:bg-white hover:text-[#1a2c4e] transition-colors duration-300 backdrop-blur-sm">
				Our work
			</a>
		</div>
	</section>

	<!-- Trusted Partners -->
	<section class="bg-[#fdfbf7] px-6 md:px-12 lg:px-24 py-16 md:py-24">
		<p class="text-lg md:text-xl text-gray-600 mb-12">Our trusted partners, from bold startups to global icons</p>
		
		<div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-6 gap-4 md:gap-8">
			<!-- Logos placeholders -->
			{#each ['etched', 'Accel', 'zid', 'gravity sketch', 'Sylvera', 'TESSIAN'] as partner}
				<div class="h-20 bg-gray-100 rounded-lg flex items-center justify-center grayscale opacity-70 hover:opacity-100 hover:grayscale-0 transition-all duration-300">
					<span class="font-semibold text-gray-800">{partner}</span>
				</div>
			{/each}
		</div>
	</section>

    <!-- Work Section -->
    <section class="bg-[#fdfbf7] px-6 md:px-12 lg:px-24 py-12 md:py-24" id="work">
        <div class="flex flex-col md:flex-row justify-between items-end mb-16 md:mb-24">
            <h2 class="font-serif text-3xl md:text-4xl lg:text-5xl text-gray-900">Our work, from petal to planet</h2>
            <a href="/work" class="hidden md:inline-flex items-center text-gray-500 hover:text-gray-900 transition-colors mt-4 md:mt-0">
                See all <span class="ml-2">→</span>
            </a>
        </div>

        <div class="space-y-24 md:space-y-32">
            <!-- Project 1: Sylvera -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Sylvera</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        Sylvera incentivises investment into real climate action by providing ratings, data, and marketing insight for over 20,000 carbon credit projects.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Brand Identity</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Digital Design</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-[#003322] rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <div class="absolute inset-0 flex items-center justify-center">
                            <div class="text-white text-3xl font-medium flex items-center gap-2">
                                <!-- Logo placeholder -->
                                <div class="w-8 h-8 rounded-full border-2 border-white/80 border-t-transparent animate-spin" style="animation-duration: 3s;"></div>
                                Sylvera
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Project 2: Knotel -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Knotel</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        Transforming the digital architecture for a modern workplace provider.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Website</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Digital Design</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-[#f5f5f0] rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <!-- Image placeholder -->
                        <img src="https://images.unsplash.com/photo-1618221195710-dd6b41faaea6?q=80&w=2000&auto=format&fit=crop" alt="Knotel interior" class="w-full h-full object-cover" />
                    </div>
                </div>
            </div>

            <!-- Project 3: Folio -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Folio</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        Folio is a digital platform designed from the ground up, helping large enterprises organise, manage and deliver design standards to streamline workflows and ensure cohesion in every project.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Brand Identity</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Digital Design</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Website</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-gray-200 rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <div class="absolute inset-0 flex items-center justify-center bg-gradient-to-br from-gray-100 to-gray-300">
                             <h4 class="text-6xl font-bold text-white drop-shadow-lg">Folio</h4>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Project 4: Printosis -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Printosis</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        Printosis is a revolutionary tool that fuses AI with orthotists using scans and patient data to generate a printable 3D model, fabricating a perfect-fit orthotic on the first attempt.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Brand Identity</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">3D Design</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-[#f0f4f0] rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out border border-gray-100">
                        <div class="absolute inset-0 flex items-center justify-center bg-[url('https://www.transparenttextures.com/patterns/graphy.png')] opacity-50"></div>
                        <div class="absolute inset-0 flex items-center justify-center">
                            <!-- Abstract shape placeholder -->
                            <div class="w-32 h-32 border border-gray-300 rounded-full skew-x-12 skew-y-12"></div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        
        <div class="mt-12 md:hidden">
            <a href="/work" class="flex items-center text-gray-500 hover:text-gray-900 transition-colors">
                See all <span class="ml-2">→</span>
            </a>
        </div>
    </section>

    <!-- Process Section -->
    <section class="bg-[#fdfbf7] px-6 md:px-12 lg:px-24 py-12 md:py-24">
        <h2 class="font-serif text-3xl md:text-4xl lg:text-5xl text-gray-900 mb-16 max-w-3xl">Our process, crafted through decades of shared experience</h2>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            <!-- Think -->
            <div class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition-shadow duration-300 flex flex-col h-full min-h-[400px]">
                <h3 class="text-xl font-semibold mb-4">Think</h3>
                <p class="text-gray-600 text-sm leading-relaxed mb-auto">
                    We read the soil to find where ideas take root, uncovering opportunities, directions, and missions.
                </p>
                <div class="mt-8 flex justify-center h-48 items-end">
                    <img src="https://images.unsplash.com/photo-1610389368568-243553229202?q=80&w=400&auto=format&fit=crop" alt="Bud" class="h-full object-contain mix-blend-multiply opacity-80" />
                </div>
            </div>

            <!-- Create -->
            <div class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition-shadow duration-300 flex flex-col h-full min-h-[400px]">
                <h3 class="text-xl font-semibold mb-4">Create</h3>
                <p class="text-gray-600 text-sm leading-relaxed mb-auto">
                    We coax the invisible into the inevitable, crafting identities and systems to support your growth.
                </p>
                <div class="mt-8 flex justify-center h-48 items-end">
                    <img src="https://images.unsplash.com/photo-1507646870321-10de075e8236?q=80&w=400&auto=format&fit=crop" alt="Blooming" class="h-full object-contain mix-blend-multiply opacity-80" />
                </div>
            </div>

            <!-- Build -->
            <div class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition-shadow duration-300 flex flex-col h-full min-h-[400px]">
                <h3 class="text-xl font-semibold mb-4">Build</h3>
                <p class="text-gray-600 text-sm leading-relaxed mb-auto">
                    We engineer scalable digital products and experiences ready for real-world impact.
                </p>
                <div class="mt-8 flex justify-center h-48 items-end">
                    <img src="https://images.unsplash.com/photo-1462275646964-a0e3386b89fa?q=80&w=400&auto=format&fit=crop" alt="Flower" class="h-full object-contain mix-blend-multiply opacity-80" />
                </div>
            </div>
        </div>
    </section>

    <!-- Thoughts Section -->
    <section class="bg-[#fdfbf7] px-6 md:px-12 lg:px-24 py-12 md:py-24">
        <div class="flex flex-col md:flex-row justify-between items-end mb-12">
            <h2 class="font-serif text-3xl md:text-4xl text-gray-900">Thoughts from our world, to yours</h2>
            <a href="/thoughts" class="hidden md:inline-flex items-center text-gray-500 hover:text-gray-900 transition-colors mt-4 md:mt-0">
                Read all <span class="ml-2">→</span>
            </a>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
            <!-- Blog Post 1 -->
            <div class="group cursor-pointer">
                <div class="aspect-square bg-gray-900 rounded-lg overflow-hidden mb-4 relative">
                     <div class="absolute inset-0 flex items-center justify-center text-white font-bold text-4xl text-center p-4">FONTS IN USE</div>
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">New Genre Featured in Fonts in Use</h3>
            </div>

             <!-- Blog Post 2 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-orange-400 rounded-lg overflow-hidden mb-4 relative">
                    <div class="absolute inset-0 flex items-center justify-center text-black font-bold text-4xl text-center p-4 rotate-12">CHILI BOMBA</div>
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">Chili Bomba Featured in Fonts in Use</h3>
            </div>

             <!-- Blog Post 3 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-green-800 rounded-lg overflow-hidden mb-4 relative">
                     <div class="absolute inset-0 flex items-center justify-center text-white text-right p-8 flex-col items-end">
                        <span class="text-sm uppercase tracking-widest mb-2">Precision</span>
                        <span class="text-2xl font-serif">at your fingertips</span>
                     </div>
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">New Identity and Website for Printosis Designed by New Genre</h3>
            </div>

             <!-- Blog Post 4 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-gray-800 rounded-lg overflow-hidden mb-4 relative">
                    <!-- Placeholder image -->
                    <img src="https://images.unsplash.com/photo-1550684848-fac1c5b4e853?q=80&w=1000&auto=format&fit=crop" alt="Office" class="w-full h-full object-cover opacity-50" />
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">New Logo and Identity for Folio by New Genre</h3>
            </div>

             <!-- Blog Post 5 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-black rounded-lg overflow-hidden mb-4 relative flex items-center justify-center">
                    <div class="w-3/4 h-3/4 bg-gray-900 rounded-3xl border border-gray-700 p-4 flex flex-col items-center justify-between">
                        <span class="text-white text-xs">9:41</span>
                        <div class="grid grid-cols-2 gap-2 w-full">
                            <div class="bg-blue-500 rounded-lg h-12"></div>
                            <div class="bg-red-500 rounded-lg h-12"></div>
                        </div>
                    </div>
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">New Genre designs identity, platform and website for new design standards tool</h3>
            </div>

             <!-- Blog Post 6 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-teal-600 rounded-lg overflow-hidden mb-4 relative">
                     <img src="https://images.unsplash.com/photo-1556761175-5973dc0f32e7?q=80&w=1000&auto=format&fit=crop" alt="Phone" class="w-full h-full object-cover mix-blend-overlay" />
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">The New Genre Studio Revamps Framework, the Challenge Platform: A Fresh Approach to...</h3>
            </div>
        </div>
    </section>

    <!-- Newsletter Section -->
    <section class="px-6 md:px-12 lg:px-24 py-12">
        <div class="bg-gradient-to-r from-[#eaddcf] to-[#e8d5c4] rounded-2xl p-8 md:p-16 lg:p-20">
            <h3 class="font-serif text-2xl md:text-3xl text-gray-900 mb-4">Get dispatches from the edge of unknown</h3>
            <p class="text-gray-600 mb-8 max-w-md">Every month, we promise to share what we're seeing, making, and thinking. Sign up if you dare.</p>
            
            <form class="flex flex-col sm:flex-row gap-4 max-w-lg">
                <input type="email" placeholder="johnnyappleseed@newgenre.studio" class="flex-1 bg-white/50 border-0 rounded-lg px-4 py-3 text-sm placeholder:text-gray-400 focus:ring-1 focus:ring-gray-400 outline-none" />
                <button type="submit" class="bg-transparent border border-gray-900/20 hover:bg-gray-900 hover:text-white transition-colors text-gray-900 px-6 py-3 rounded-lg text-sm font-medium">
                    Sign me up
                </button>
            </form>
            <p class="text-[10px] text-gray-500 mt-4">We'll never share your details. By signing up, you agree to receive communications from New Genre. Read our Privacy Policy.</p>
        </div>
    </section>

    <!-- Constellations (Footer Hero) -->
    <section class="relative bg-gradient-to-b from-[#e69d75] via-[#c46d5e] to-[#8b3a2b] pt-32 pb-48 px-6 md:px-12 lg:px-24 overflow-hidden">
        <div class="max-w-5xl relative z-10">
            <h2 class="font-serif text-4xl md:text-6xl lg:text-7xl text-[#fdfbf7] leading-tight mb-8">
                All our constellations, under one sky. <br />
                <span class="text-[#fdfbf7]/70">Find out how we chart the path from idea to icon — through strategy, creation, building, and scaling — turning the unseeable into the undeniable.</span>
            </h2>
            
            <div class="mt-16">
                 <a href="/approach" class="inline-flex items-center justify-center px-6 py-3 border border-white/30 rounded-full text-sm font-medium text-white hover:bg-white hover:text-[#8b3a2b] transition-colors duration-300 backdrop-blur-sm">
                    Our Approach
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-[#3e1c16] text-[#eaddcf] px-6 md:px-12 lg:px-24 pt-24 pb-12 relative overflow-hidden">
        
        <!-- Large Flower Image Overlapping Sections -->
        <div class="absolute bottom-0 left-1/2 transform -translate-x-1/2 translate-y-0 w-[800px] h-[1000px] pointer-events-none z-0 opacity-90 mix-blend-hard-light">
             <img src="https://images.unsplash.com/photo-1596294399224-b174780e816e?q=80&w=1000&auto=format&fit=crop" alt="Hibiscus Flower" class="w-full h-full object-contain" />
        </div>

        <div class="relative z-10">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-12 mb-24">
                <div class="col-span-1 md:col-span-2">
                    <a href="/contact" class="text-2xl font-medium hover:opacity-80 transition-opacity inline-flex items-center">
                        Work with us <span class="ml-2">→</span>
                    </a>
                </div>
                
                <div class="space-y-4">
                    <h4 class="font-medium text-white">London, UK</h4>
                    <p class="text-sm opacity-70">5:20 am</p>
                    <div class="pt-4 text-sm opacity-70 space-y-1">
                        <p>london@newgenre.studio</p>
                        <p>+44 20 4572 6788</p>
                        <p class="mt-4">2 Appleby Yard,<br>Seames Walk,<br>London SE10 0BU, UK</p>
                    </div>
                </div>

                <div class="space-y-4">
                    <h4 class="font-medium text-white">San Francisco</h4>
                    <p class="text-sm opacity-70">9:20 pm</p>
                    <div class="pt-4 text-sm opacity-70 space-y-1">
                        <p>sf@newgenre.studio</p>
                        <p>+1 650 466 6274</p>
                    </div>
                </div>
            </div>

            <div class="flex flex-col md:flex-row justify-between items-end border-t border-white/10 pt-8">
                <div class="mb-4 md:mb-0">
                    <!-- Logo Icon -->
                    <svg width="32" height="32" viewBox="0 0 24 24" fill="currentColor" class="text-white">
                        <rect x="2" y="2" width="9" height="9" rx="2" />
                        <rect x="13" y="2" width="9" height="9" rx="2" />
                        <rect x="2" y="13" width="9" height="9" rx="2" />
                        <rect x="13" y="13" width="9" height="9" rx="2" />
                    </svg>
                </div>
                
                <div class="flex gap-6 text-xs font-medium">
                    <a href="#" class="hover:text-white transition-colors">LinkedIn</a>
                    <a href="#" class="hover:text-white transition-colors">Instagram</a>
                    <a href="#" class="hover:text-white transition-colors">X</a>
                    <a href="#" class="hover:text-white transition-colors">Join Us</a>
                </div>
            </div>

            <div class="flex justify-between text-[10px] opacity-50 mt-12">
                <p>© 2025 New Genre</p>
                <p>Privacy</p>
            </div>
        </div>
    </footer>
</div>

<style>
    /* Custom utility for vertical writing mode */
    .writing-vertical-rl {
        writing-mode: vertical-rl;
    }
</style>

