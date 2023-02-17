<script lang="ts">
	const features = [
		{
			title: 'Design',
			icon: 'upload',
			description:
				'Wordpress, Photoshop, Canva'
		},
		// {
		// 	title: 'Stream On-Demand',
		// 	icon: 'record',
		// 	description: 'Showcase your content in a beautiful on-demand video catalog.'
		// },
		// {
		// 	title: 'Stream live',
		// 	icon: 'stream',
		// 	description: 'Schedule events in advance & build excitement with a countdown overlay.'
		// },
		// {
		// 	title: 'Monetization',
		// 	icon: 'monetization',
		// 	description: 'Offer subscriptions or one-time purchases. Accept credit cards & PayPal.'
		// },
		{
			title: 'Analytics',
			icon: 'stream',
			description: 'Data science'
		},
		{
			title: 'Developer',
			icon: 'device',
			description: 'Html, Css, JavaScript, React, Flutter'
		}
	]
</script>

<section class="py-10 text-black bg-white ml-10">
	<div class="max-w-screen-xl mx-auto">
		<div class="flex items-center space-x-24">
			<div class="flex flex-col w-1/2">
				<div class="flex flex-col space-y-4">
					<h1 class="text-5xl font-bold font-heading">Hey I'm</h1>
					<h1 class="text-5xl font-bold font-heading">Marwan</h1>
					<p>
						Frontend Developer with intermediate level of experience in web designing
            and development.
					</p>
				</div>
				<div class="w-10 flex mt-32 space-x-24 items-center">
				<img
				src="/images/github.png"
				class="transform transition duration-300 hover:scale-110 cursor-pointer"
				alt="Apple TV"
			/>
			<img
				src="/images/linkedin.png"
				class="transform transition duration-300 hover:scale-110 cursor-pointer"
				alt="Android TV"
			/>
			<img
				src="/images/facebook.png"
				class="transform transition duration-300 hover:scale-110 cursor-pointer"
				alt="Apple Watch"
			/> 
		</div>
				<!-- <div class="flex mt-12 space-x-3">
					<button class="w-1/3 primary">Start Free Trial</button>
					<button class="w-1/3 outline">Login</button>
				</div> -->
			</div>
			<div class="relative w-1/2 bprder border-solid border-red-800 rounded-lg">
				<img src="/images/me.jpg" class="w-full h-96 max-w-sm rounded-lg shadow-2xl" alt="Hero" />
				<!-- <img src="/images/hero-image-mobile.png" class="absolute -bottom-4 -left-3" alt="Hero" /> -->
			</div>
		    
		</div>
		<div class="w-10 flex mt-32 space-x-24 items-center">
			
			<!-- <img
				src="/images/iphone.svg"
				class="transform transition duration-300 hover:scale-110 cursor-pointer"
				alt="iPhone"
			/>
			<img
				src="/images/android.svg"
				class="transform transition duration-300 hover:scale-110 cursor-pointer"
				alt="Android"
			/> -->
		</div>
	</div>
</section>
<!-- <div class="hero min-h-screen bg-base-200">
	<div class="hero-content flex-col lg:flex-row-reverse">
	  <img src="/images/me.jpg" class="max-w-sm rounded-lg shadow-2xl" />
	  <div>
		<h1 class="text-5xl font-bold">Box Office News!</h1>
		<p class="py-6">Provident cupiditate voluptatem et in. Quaerat fugiat ut assumenda excepturi exercitationem quasi. In deleniti eaque aut repudiandae et a id nisi.</p>
		<button class="btn btn-primary">Get Started</button>
	  </div>
	</div>
  </div> -->

<section class="py-20 bg-white text-black" id="service">
	<div class="max-w-screen-lg mx-auto">
		<div class="flex flex-col justify-center text-center">
			<div class="flex flex-col space-y-3">
				<h2 class="text-4xl font-bold font-heading">Services</h2>
				<p>Below are the services i provide</p>
			</div>
			
		</div>
		<div class="grid grid-cols-3 gap-12 mt-20">
			{#each features as feature}
				<div
					class="flex flex-col p-4 space-y-3 hover:shadow-2xl transition duration-300 cursor-pointer"
				>
					<div class="flex space-x-3">
						<img
							src={`/icons/${feature.icon}.svg`}
							class="transform transition duration-300 hover:rotate-12"
							alt={feature.title}
						/>
						<h5 class="font-bold font-heading">{feature.title}</h5>
					</div>
					<p>{feature.description}</p>
				</div>
			{/each}
		</div>
	</div>
</section>

<!-- <section class="py-20 text-white bg-black">
	<div class="flex flex-col max-w-screen-xl mx-auto space-y-32">
		<div class="flex flex-col justify-center">
			<h2 class="text-4xl font-bold text-center font-heading">We help you grow</h2>
		</div>

		<div class="flex space-x-24">
			<div class="flex flex-col justify-center w-1/2 space-y-6">
				<h5 class="text-3xl font-semibold">Monetize your way</h5>
				<p>
					Set up subscriptions, rentals, or one-time buys for access to your VOD and live streams.
					Create exclusive experiences for your subscribers with coupons and promotions. One
					predictable fee, transparent pricing, and same-day setup.
				</p>
				<div class="flex space-x-3 cursor-pointer group">
					<p class="transition font-heading group-hover:font-bold">Get started</p>
					<img
						src="/icons/arrow.svg"
						class="transition transform group-hover:translate-x-1"
						alt="Arrow Icon"
					/>
				</div>
			</div>
			<div class="relative w-1/2">
				<img src="/images/monetization.png" alt="Monetize your way" class="w-full h-full" />
				<div
					class="absolute flex flex-col py-8 space-y-3 text-black bg-white px-9 rounded-3xl -top-4 -left-6"
				>
					<div
						class="flex w-full px-3 py-4 space-x-16 font-semibold transition duration-300 transform bg-gray-100 font-heading rounded-xl hover:bg-blue-100 hover:text-primary hover:translate-x-1 hover:-translate-y-1 hover:shadow-xl"
					>
						<p>Donate</p>
						<p>45$</p>
					</div>
					<div
						class="flex w-full px-3 py-4 space-x-16 font-semibold transition duration-300 transform bg-gray-100 font-heading rounded-xl hover:bg-blue-100 hover:text-primary hover:translate-x-1 hover:-translate-y-1 hover:shadow-xl"
					>
						<p>Donate</p>
						<p>45$</p>
					</div>
					<div
						class="flex w-full px-3 py-4 space-x-16 font-semibold transition duration-300 transform bg-gray-100 font-heading rounded-xl hover:bg-blue-100 hover:text-primary hover:translate-x-1 hover:-translate-y-1 hover:shadow-xl"
					>
						<p>Donate</p>
						<p>45$</p>
					</div>
				</div>
			</div>
		</div>

		<div class="flex space-x-24">
			<div class="relative flex w-1/2">
				<img src="/images/optimized.png" class="w-full h-full" alt="Optimized for growth" />
				<div class="absolute px-4 py-3 bg-white -top-4 -right-4 rounded-2xl">
					<div class="relative">
						<img src="/icons/email-black.svg" alt="Email Icon" class="w-8 h-6" />
						<span
							class="absolute text-xs rounded-full -top-2 -right-2 bg-primary px-[6px] py-[1px] font-heading font-bold"
							>1</span
						>
					</div>
				</div>
			</div>
			<div class="flex flex-col justify-center w-1/2 space-y-6">
				<h5 class="text-3xl font-semibold">Optimized for growth</h5>
				<p>
					The Screeno ecosystem is designed to help you generate profit. Set up complete sales and
					marketing funnels with ease using the Screeno built-in marketing tools and integrations.
					Generate leads and convert your audience into paying subscribers, at no extra cost.
				</p>
				<div class="flex space-x-3 cursor-pointer group">
					<p class="transition font-heading group-hover:font-bold">Get started</p>
					<img
						src="/icons/arrow.svg"
						class="transition transform group-hover:translate-x-1"
						alt="Arrow Icon"
					/>
				</div>
			</div>
		</div>
	</div>
</section> -->

<!-- <section class="pt-20 pb-40 text-white bg-black">
	<div class="flex flex-col max-w-screen-lg mx-auto">
		<div class="flex flex-col space-y-3 text-center">
			<h2 class="text-4xl font-bold font-heading">Start your own business today</h2>
			<p>Consistent quality and experience across all platforms and devices.</p>
		</div>
		<div class="flex justify-center space-x-8 mt-14">
			<button class="w-1/5 secondary">Get started</button>
			<button class="w-1/5 outline">Login</button>
		</div>
		<div class="relative mt-20">
			<img src="/images/business-desktop.png" alt="Business Desktop" class="w-full h-full" />
			<img
				src="/images/business-mobile.png"
				alt="Business Mobile"
				class="absolute -bottom-12 -left-3"
			/>
		</div>
	</div>
</section> -->

<section class="pt-20 pb-32 bg-black text-white">
	<div class="flex flex-col justify-center space-y-3 text-center">
		<h2 class="text-4xl font-bold font-heading">Portfolio</h2>
		<p>Recent Projects</p>
	</div>

	<div class="flex flex-col overflow-hidden mt-24 space-y-6 items-center">
		<div class="flex space-x-8 shadow-xl">
			<img src="/images/ayabooks.png" alt="Showcase 1" class="w-[360px] h-[201px] rounded-lg" />
			<img src="/images/phm.png" alt="Showcase 2" class="w-[360px] h-[201px] rounded-lg " />
			<!-- <img src="/images/showcase-3.png" alt="Showcase 3" class="w-[360px] h-[201px]" />
			<img src="/images/showcase-4.png" alt="Showcase 4" class="w-[360px] h-[201px]" /> -->
		</div>
		<!-- <div class="flex space-x-8 -translate-x-72">
			<img src="/images/showcase-5.png" alt="Showcase 5" class="w-[360px] h-[201px]" />
			<img src="/images/showcase-6.png" alt="Showcase 6" class="w-[360px] h-[201px]" />
			<img src="/images/showcase-7.png" alt="Showcase 7" class="w-[360px] h-[201px]" />
			<img src="/images/showcase-8.png" alt="Showcase 8" class="w-[360px] h-[201px]" />
			<img src="/images/showcase-9.png" alt="Showcase 9" class="w-[360px] h-[201px]" />
		</div> -->
	</div>
</section>
