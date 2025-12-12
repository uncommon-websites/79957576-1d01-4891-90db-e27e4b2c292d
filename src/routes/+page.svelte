<script lang="ts">
	import { onMount } from 'svelte';

	let scrollY = 0;
</script>

<svelte:head>
	<title>TOP G - Premium Lifestyle Brand for Men</title>
	<meta name="description" content="Elevate your status with TOP G. Premium merchandise, performance supplements, and exclusive collectibles for men who demand excellence." />
</svelte:head>

<svelte:window bind:scrollY />

<div class="font-sans text-gray-900 antialiased selection:bg-primary-200 selection:text-primary-900">
	<!-- Hero Section -->
	<section class="relative min-h-screen w-full bg-gradient-to-b from-black via-gray-900 to-gray-100 text-white px-6 md:px-12 lg:px-24 pt-32 pb-24 flex flex-col justify-between">
		<div class="max-w-5xl">
			<h1 class="font-serif text-5xl md:text-7xl lg:text-8xl leading-[1.1] md:leading-[1.1] tracking-tight">
				Elevate Your Status. Dominate Your Life. Live Like a TOP G.
			</h1>
			<p class="mt-8 text-xl md:text-2xl text-gray-300 max-w-3xl">
				Premium lifestyle brand for men who refuse to settle. Exclusive merchandise, performance supplements, and collectibles for those who demand excellence.
			</p>
		</div>

		<div class="mt-24">
			<a href="#collections" class="inline-flex items-center justify-center px-8 py-4 bg-primary-600 hover:bg-primary-700 rounded-full text-sm font-bold uppercase tracking-wider transition-colors duration-300">
				Shop Collections
			</a>
		</div>
	</section>

	<!-- Social Proof -->
	<section class="bg-white px-6 md:px-12 lg:px-24 py-16 md:py-24">
		<p class="text-lg md:text-xl text-gray-600 mb-12 text-center">Join 100,000+ men who've elevated their lifestyle</p>
		
		<div class="grid grid-cols-2 md:grid-cols-4 gap-8 md:gap-12 max-w-4xl mx-auto">
			<div class="text-center">
				<div class="text-4xl md:text-5xl font-bold text-black mb-2">100K+</div>
				<div class="text-sm text-gray-600 uppercase tracking-wider">Customers</div>
			</div>
			<div class="text-center">
				<div class="text-4xl md:text-5xl font-bold text-black mb-2">50+</div>
				<div class="text-sm text-gray-600 uppercase tracking-wider">Products</div>
			</div>
			<div class="text-center">
				<div class="text-4xl md:text-5xl font-bold text-black mb-2">4.9★</div>
				<div class="text-sm text-gray-600 uppercase tracking-wider">Rating</div>
			</div>
			<div class="text-center">
				<div class="text-4xl md:text-5xl font-bold text-black mb-2">24/7</div>
				<div class="text-sm text-gray-600 uppercase tracking-wider">Support</div>
			</div>
		</div>
	</section>

    <!-- Collections Section -->
    <section class="bg-gray-50 px-6 md:px-12 lg:px-24 py-12 md:py-24" id="collections">
        <div class="flex flex-col md:flex-row justify-between items-end mb-16 md:mb-24">
            <h2 class="font-serif text-3xl md:text-4xl lg:text-5xl text-gray-900">Premium Collections</h2>
            <a href="/shop" class="hidden md:inline-flex items-center text-gray-500 hover:text-gray-900 transition-colors mt-4 md:mt-0">
                Shop all <span class="ml-2">→</span>
            </a>
        </div>

        <div class="space-y-24 md:space-y-32">
            <!-- Collection 1: Merchandise -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Premium Merchandise</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        Exclusive apparel and accessories designed for men who demand the best. Limited edition pieces that make a statement and command respect.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 bg-black text-white rounded-full text-xs font-medium uppercase">Apparel</span>
                        <span class="px-3 py-1 bg-black text-white rounded-full text-xs font-medium uppercase">Accessories</span>
                        <span class="px-3 py-1 bg-black text-white rounded-full text-xs font-medium uppercase">Limited Edition</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-black rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <img src="https://images.unsplash.com/photo-1556821840-3a63f95609a7?q=80&w=2000&auto=format&fit=crop" alt="Premium merchandise" class="w-full h-full object-cover opacity-80" />
                        <div class="absolute inset-0 bg-gradient-to-t from-black/60 to-transparent"></div>
                    </div>
                </div>
            </div>

            <!-- Collection 2: Supplements -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Performance Supplements</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        Premium formulations engineered for peak performance. Fuel your body with supplements designed for champions who refuse to compromise.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 bg-black text-white rounded-full text-xs font-medium uppercase">Pre-Workout</span>
                        <span class="px-3 py-1 bg-black text-white rounded-full text-xs font-medium uppercase">Protein</span>
                        <span class="px-3 py-1 bg-black text-white rounded-full text-xs font-medium uppercase">Recovery</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-gray-900 rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <img src="https://images.unsplash.com/photo-1593095948071-474c5cc2989d?q=80&w=2000&auto=format&fit=crop" alt="Performance supplements" class="w-full h-full object-cover opacity-70" />
                        <div class="absolute inset-0 bg-gradient-to-t from-black/60 to-transparent"></div>
                    </div>
                </div>
            </div>

            <!-- Collection 3: Collectibles -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Exclusive Collectibles</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        Limited edition items and luxury accessories that define status. Own pieces that separate you from the crowd and showcase your success.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 bg-black text-white rounded-full text-xs font-medium uppercase">Limited Run</span>
                        <span class="px-3 py-1 bg-black text-white rounded-full text-xs font-medium uppercase">Numbered</span>
                        <span class="px-3 py-1 bg-black text-white rounded-full text-xs font-medium uppercase">Premium</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-gray-800 rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <img src="https://images.unsplash.com/photo-1523170335258-f5ed11844a49?q=80&w=2000&auto=format&fit=crop" alt="Luxury collectibles" class="w-full h-full object-cover opacity-75" />
                        <div class="absolute inset-0 bg-gradient-to-t from-black/60 to-transparent"></div>
                    </div>
                </div>
            </div>
        </div>
        
        <div class="mt-12 md:hidden">
            <a href="/shop" class="flex items-center text-gray-500 hover:text-gray-900 transition-colors">
                Shop all <span class="ml-2">→</span>
            </a>
        </div>
    </section>

    <!-- Values Section -->
    <section class="bg-white px-6 md:px-12 lg:px-24 py-12 md:py-24">
        <h2 class="font-serif text-3xl md:text-4xl lg:text-5xl text-gray-900 mb-16 max-w-3xl">The TOP G Way: Excellence, Success, Brotherhood</h2>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            <!-- Excellence -->
            <div class="bg-black text-white p-8 rounded-xl hover:scale-[1.02] transition-transform duration-300 flex flex-col h-full min-h-[400px]">
                <h3 class="text-2xl font-bold mb-4 uppercase tracking-wider">Excellence</h3>
                <p class="text-gray-300 text-sm leading-relaxed mb-auto">
                    We don't do average. Every product, every detail is crafted to the highest standard. Mediocrity is not an option.
                </p>
                <div class="mt-8 flex justify-center h-48 items-center">
                    <img src="https://images.unsplash.com/photo-1534438327276-14e5300c3a48?q=80&w=400&auto=format&fit=crop" alt="Excellence" class="w-full h-full object-cover rounded-lg opacity-80" />
                </div>
            </div>

            <!-- Success -->
            <div class="bg-black text-white p-8 rounded-xl hover:scale-[1.02] transition-transform duration-300 flex flex-col h-full min-h-[400px]">
                <h3 class="text-2xl font-bold mb-4 uppercase tracking-wider">Success</h3>
                <p class="text-gray-300 text-sm leading-relaxed mb-auto">
                    Built by winners, for winners. We celebrate achievement and provide the tools you need to dominate in every aspect of life.
                </p>
                <div class="mt-8 flex justify-center h-48 items-center">
                    <img src="https://images.unsplash.com/photo-1551836022-d5d88e9218df?q=80&w=400&auto=format&fit=crop" alt="Success" class="w-full h-full object-cover rounded-lg opacity-80" />
                </div>
            </div>

            <!-- Brotherhood -->
            <div class="bg-black text-white p-8 rounded-xl hover:scale-[1.02] transition-transform duration-300 flex flex-col h-full min-h-[400px]">
                <h3 class="text-2xl font-bold mb-4 uppercase tracking-wider">Brotherhood</h3>
                <p class="text-gray-300 text-sm leading-relaxed mb-auto">
                    Join an exclusive community of high-achievers. Network with men who share your drive and ambition.
                </p>
                <div class="mt-8 flex justify-center h-48 items-center">
                    <img src="https://images.unsplash.com/photo-1511632765486-a01980e01a18?q=80&w=400&auto=format&fit=crop" alt="Brotherhood" class="w-full h-full object-cover rounded-lg opacity-80" />
                </div>
            </div>
        </div>
    </section>

    <!-- Lifestyle Content Section -->
    <section class="bg-gray-50 px-6 md:px-12 lg:px-24 py-12 md:py-24">
        <div class="flex flex-col md:flex-row justify-between items-end mb-12">
            <h2 class="font-serif text-3xl md:text-4xl text-gray-900">Lifestyle & Mindset</h2>
            <a href="/blog" class="hidden md:inline-flex items-center text-gray-500 hover:text-gray-900 transition-colors mt-4 md:mt-0">
                Read all <span class="ml-2">→</span>
            </a>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
            <!-- Blog Post 1 -->
            <div class="group cursor-pointer">
                <div class="aspect-square bg-black rounded-lg overflow-hidden mb-4 relative">
                     <img src="https://images.unsplash.com/photo-1571019613454-1cb2f99b2d8b?q=80&w=1000&auto=format&fit=crop" alt="Business success" class="w-full h-full object-cover opacity-70" />
                     <div class="absolute inset-0 flex items-center justify-center text-white font-bold text-2xl text-center p-4 bg-black/40">BUILD YOUR EMPIRE</div>
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">10 Rules for Building a Million Dollar Business</h3>
            </div>

             <!-- Blog Post 2 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-gray-900 rounded-lg overflow-hidden mb-4 relative">
                    <img src="https://images.unsplash.com/photo-1517836357463-d25dfeac3438?q=80&w=1000&auto=format&fit=crop" alt="Fitness" class="w-full h-full object-cover opacity-70" />
                    <div class="absolute inset-0 flex items-center justify-center text-white font-bold text-2xl text-center p-4 bg-black/40">PEAK PERFORMANCE</div>
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">The Ultimate Guide to Building an Alpha Physique</h3>
            </div>

             <!-- Blog Post 3 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-gray-800 rounded-lg overflow-hidden mb-4 relative">
                     <img src="https://images.unsplash.com/photo-1507679799987-c73779587ccf?q=80&w=1000&auto=format&fit=crop" alt="Success mindset" class="w-full h-full object-cover opacity-70" />
                     <div class="absolute inset-0 flex items-center justify-center text-white font-bold text-2xl text-center p-4 bg-black/40">MINDSET MASTERY</div>
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">How to Develop an Unbreakable Winner's Mindset</h3>
            </div>

             <!-- Blog Post 4 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-black rounded-lg overflow-hidden mb-4 relative">
                    <img src="https://images.unsplash.com/photo-1549576490-b0b4831ef60a?q=80&w=1000&auto=format&fit=crop" alt="Luxury lifestyle" class="w-full h-full object-cover opacity-70" />
                    <div class="absolute inset-0 flex items-center justify-center text-white font-bold text-2xl text-center p-4 bg-black/40">LUXURY LIVING</div>
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">Essential Status Symbols Every TOP G Should Own</h3>
            </div>

             <!-- Blog Post 5 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-gray-900 rounded-lg overflow-hidden mb-4 relative">
                    <img src="https://images.unsplash.com/photo-1552581234-26160f608093?q=80&w=1000&auto=format&fit=crop" alt="Networking" class="w-full h-full object-cover opacity-70" />
                    <div class="absolute inset-0 flex items-center justify-center text-white font-bold text-2xl text-center p-4 bg-black/40">NETWORK POWER</div>
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">How to Network Like a High-Value Male</h3>
            </div>

             <!-- Blog Post 6 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-black rounded-lg overflow-hidden mb-4 relative">
                     <img src="https://images.unsplash.com/photo-1590650153855-d9e808231d41?q=80&w=1000&auto=format&fit=crop" alt="Style" class="w-full h-full object-cover opacity-70" />
                     <div class="absolute inset-0 flex items-center justify-center text-white font-bold text-2xl text-center p-4 bg-black/40">STYLE GUIDE</div>
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">Dressing for Success: The TOP G Style Manual</h3>
            </div>
        </div>
    </section>

    <!-- Newsletter Section -->
    <section class="px-6 md:px-12 lg:px-24 py-12">
        <div class="bg-gradient-to-r from-black to-gray-900 rounded-2xl p-8 md:p-16 lg:p-20">
            <h3 class="font-serif text-2xl md:text-3xl text-white mb-4">Join the Elite Circle</h3>
            <p class="text-gray-300 mb-8 max-w-md">Get exclusive access to new drops, lifestyle tips, and members-only content. Elevate your game.</p>
            
            <form class="flex flex-col sm:flex-row gap-4 max-w-lg">
                <input type="email" placeholder="your@email.com" class="flex-1 bg-white/10 border border-white/20 rounded-lg px-4 py-3 text-sm placeholder:text-gray-400 text-white focus:ring-2 focus:ring-primary-500 outline-none" />
                <button type="submit" class="bg-primary-600 hover:bg-primary-700 transition-colors text-white px-8 py-3 rounded-lg text-sm font-bold uppercase tracking-wider">
                    Join Now
                </button>
            </form>
            <p class="text-[10px] text-gray-400 mt-4">We respect your privacy. By signing up, you agree to receive communications from TOP G. Read our Privacy Policy.</p>
        </div>
    </section>

    <!-- CTA Hero Section -->
    <section class="relative bg-gradient-to-b from-gray-900 via-black to-gray-900 pt-32 pb-48 px-6 md:px-12 lg:px-24 overflow-hidden">
        <div class="max-w-5xl relative z-10">
            <h2 class="font-serif text-4xl md:text-6xl lg:text-7xl text-white leading-tight mb-8">
                Ready to Join the Elite? <br />
                <span class="text-gray-400">Stop settling for average. Start living like a TOP G. Exclusive products for men who demand excellence.</span>
            </h2>
            
            <div class="mt-16 flex flex-col sm:flex-row gap-4">
                 <a href="/shop" class="inline-flex items-center justify-center px-8 py-4 bg-primary-600 hover:bg-primary-700 rounded-full text-sm font-bold uppercase tracking-wider text-white transition-colors duration-300">
                    Shop Now
                </a>
                 <a href="/about" class="inline-flex items-center justify-center px-8 py-4 border border-white/30 rounded-full text-sm font-bold uppercase tracking-wider text-white hover:bg-white hover:text-black transition-colors duration-300">
                    Our Story
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-black text-gray-300 px-6 md:px-12 lg:px-24 pt-24 pb-12 relative overflow-hidden">
        <div class="relative z-10">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-12 mb-24">
                <div class="col-span-1 md:col-span-2">
                    <h3 class="text-3xl font-bold text-white mb-4">TOP G</h3>
                    <p class="text-gray-400 mb-6 max-w-md">Premium lifestyle brand for men who refuse to settle. Elevate your status, dominate your life.</p>
                    <a href="/contact" class="text-lg font-medium text-white hover:text-primary-500 transition-colors inline-flex items-center">
                        Get in touch <span class="ml-2">→</span>
                    </a>
                </div>
                
                <div class="space-y-4">
                    <h4 class="font-bold text-white uppercase tracking-wider text-sm">Shop</h4>
                    <div class="space-y-2 text-sm">
                        <p><a href="/merchandise" class="hover:text-white transition-colors">Merchandise</a></p>
                        <p><a href="/supplements" class="hover:text-white transition-colors">Supplements</a></p>
                        <p><a href="/collectibles" class="hover:text-white transition-colors">Collectibles</a></p>
                        <p><a href="/new" class="hover:text-white transition-colors">New Arrivals</a></p>
                    </div>
                </div>

                <div class="space-y-4">
                    <h4 class="font-bold text-white uppercase tracking-wider text-sm">Company</h4>
                    <div class="space-y-2 text-sm">
                        <p><a href="/about" class="hover:text-white transition-colors">About Us</a></p>
                        <p><a href="/blog" class="hover:text-white transition-colors">Blog</a></p>
                        <p><a href="/contact" class="hover:text-white transition-colors">Contact</a></p>
                        <p><a href="/support" class="hover:text-white transition-colors">Support</a></p>
                    </div>
                </div>
            </div>

            <div class="flex flex-col md:flex-row justify-between items-center border-t border-white/10 pt-8">
                <div class="mb-4 md:mb-0">
                    <!-- Logo Icon -->
                    <svg width="32" height="32" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="text-white">
                        <path
                            fill-rule="evenodd"
                            clip-rule="evenodd"
                            d="M10.1214 2.40967C11.0087 2.40967 11.7683 3.04566 11.9242 3.91908L12.1482 5.17341C12.3042 6.04681 13.0638 6.68282 13.951 6.68282H15.47C17.83 6.68282 19.7432 8.59595 19.7432 10.9559C19.7432 12.3696 19.0567 13.6229 17.999 14.4007C18.4424 14.5514 18.7925 14.7906 19.0496 15.1048C19.3141 15.4514 19.5031 15.9439 19.6165 16.5641C19.6354 16.7283 19.6591 16.8879 19.6827 17.0475C19.7063 17.2071 19.7299 17.3667 19.7488 17.5309C19.7685 17.7014 19.783 17.8473 19.7951 17.9686C19.8062 18.0809 19.8153 18.1721 19.8244 18.2423C19.8622 18.7531 19.9189 19.1726 19.9945 19.4827C20.0742 19.9188 20.2352 20.3438 20.4633 20.7231H17.2352C17.084 20.4313 16.9895 20.0847 16.9139 19.7016C16.8489 19.3722 16.7979 18.9617 16.7368 18.4704C16.7268 18.3904 16.7166 18.3083 16.706 18.2241L16.5926 17.385C16.4981 16.7465 16.3847 16.2905 16.2713 15.9986C16.139 15.725 15.9312 15.5244 15.6476 15.4149C15.3453 15.3055 14.8917 15.2291 14.2491 15.2291H14.1037C13.2164 15.2291 12.4568 14.5931 12.3009 13.7197L12.0769 12.4653C11.9209 11.5919 11.1613 10.9559 10.274 10.9559H7.53417V15.8395H4.48193V2.40967H10.1214ZM16.6909 10.9559C16.6909 11.6302 16.1443 12.1769 15.47 12.1769H13.951C13.0638 12.1769 12.3042 11.5408 12.1482 10.6674L11.9242 9.41312C11.7683 8.53971 11.0087 7.9037 10.1214 7.9037H7.53417V5.46189H10.274C11.1613 5.46189 11.9209 6.0979 12.0769 6.97131L12.3008 8.22563C12.4568 9.09904 13.2164 9.73505 14.1037 9.73505H15.47C16.1443 9.73505 16.6909 10.2817 16.6909 10.9559Z"
                            fill="currentColor"
                        />
                    </svg>
                </div>
                
                <div class="flex gap-6 text-xs font-medium uppercase tracking-wider">
                    <a href="https://instagram.com" target="_blank" class="hover:text-white transition-colors">Instagram</a>
                    <a href="https://twitter.com" target="_blank" class="hover:text-white transition-colors">Twitter</a>
                    <a href="https://youtube.com" target="_blank" class="hover:text-white transition-colors">YouTube</a>
                    <a href="https://tiktok.com" target="_blank" class="hover:text-white transition-colors">TikTok</a>
                </div>
            </div>

            <div class="flex flex-col md:flex-row justify-between text-[10px] opacity-50 mt-12 gap-4">
                <p>© 2025 TOP G. All rights reserved.</p>
                <div class="flex gap-4">
                    <a href="/privacy" class="hover:opacity-100 transition-opacity">Privacy Policy</a>
                    <a href="/terms" class="hover:opacity-100 transition-opacity">Terms of Service</a>
                </div>
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

