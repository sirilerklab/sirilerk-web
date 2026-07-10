<script lang="ts">
	const items = [
        {
			url: 'https://github.com/sirilerklab/svcgeyser',
			title: 'svcgeyser',
			description: '🎙️ Enables Bedrock players to use Simple Voice Chat on PaperMC servers via Geyser & Floodgate.'
		},
        {
			url: 'https://github.com/sirilerklab/vite-plugin-openobserve-sourcemap',
			title: 'vite-plugin-openobserve-sourcemap',
			description: 'Vite plugin for auto-upload sourcemap into openobserve'
		},
		{
			url: 'https://github.com/mrwan2546/tools',
			title: 'tools',
			description: 'The web-tool for any generate. It\'s simple but powerful 🔥'
		},
		{
			url: 'https://github.com/mrwan2546/promptparse-py',
			title: 'promptparse-py',
			description: 'All-in-one Python for PromptPay & EMVCo QR Codes'
		},
		{
			url: 'https://github.com/mrwan2546/promptparse-go',
			title: 'promptparse-go',
			description: 'All-in-one Golang for PromptPay & EMVCo QR Codes'
		},
		{
			url: 'https://github.com/mrwan2546/storeapi',
			title: 'storeapi',
			description: ''
		},
		{
			url: 'https://github.com/mrwan2546/cakulabruh',
			title: 'cakulabruh',
			description: 'Full caculator with arithmetic expression algorithm'
		},
		{
			url: 'https://github.com/mrwan2546/file-encryption',
			title: 'file-encryption',
			description: 'Encrypt & decrypt file with any extension'
		},
		{
			url: 'https://github.com/mrwan2546/EnkaNetwork.py',
			title: 'EnkaNetwork.py',
			description: 'Library for fetching JSON data from site https://enka.network/ with Python'
		},
		{
			url: 'https://github.com/mrwan2546/cfpage',
			title: 'cfpage',
			description: 'A simple for deploy Cloudflare page with custom data in .env file'
		},
		{
			url: 'https://github.com/mrwan2546/pyinitgen',
			title: 'pyinitgen',
			description: 'A CLI generate init python'
		},
		{
			url: 'https://github.com/mrwan2546/FishTerm',
			title: 'FishTerm',
			description: 'A open-soruce Terminal remote access'
		},
		{
			url: 'https://github.com/mrwan2546/RenderPage',
			title: 'RenderPage',
			description: 'Pre-render page smailer like prerender.io'
		},
		{
			url: 'https://github.com/mrwan2546/VTracker-Event-Stream-TS',
			title: 'VTracker-Event-Stream-TS',
			description: ''
		},
		{
			url: 'https://github.com/mrwan2546/Discord-Tech-Talk',
			title: 'Discord-Tech-Talk',
			description: 'Bot discord for make tech-talk like clubhouse but you can not to verify community discord server.'
		}
	];
</script>

<div class="container mx-auto">
	<div class="mt-6 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
		{#each items as item}
			<a
				href={item.url}
				aria-label={`Showcase ${item.title}, ${item.description} url.`}
				class="bg-white/5 p-5 flex flex-row gap-3 rounded-md scale-100 hover:scale-[1.02] duration-300 drop-shadow-none hover:drop-shadow-md drop-shadow-white"
			>
				<svg
					xmlns="http://www.w3.org/2000/svg"
					viewBox="0 0 24 24"
					fill="none"
					stroke="currentColor"
					stroke-width="2"
					stroke-linecap="round"
					stroke-linejoin="round"
					class="w-[32px] text-white"
				>
					<line x1="6" x2="6" y1="3" y2="15" /><circle cx="18" cy="6" r="3" /><circle
						cx="6"
						cy="18"
						r="3"
					/>
					<path d="M18 9a9 9 0 0 1-9 9" />
				</svg>
				<div class="text-white">
					<h1 class="font-bold text-lg">{item.title}</h1>
					<p class="text-sm">{item.description || '-'}</p>
				</div>
			</a>
		{/each}
	</div>
</div>
