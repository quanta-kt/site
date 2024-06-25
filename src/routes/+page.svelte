<script lang="ts">
	import Navbar from '$lib/components/Navbar.svelte';

	const socials = [
		{
			name: 'GitHub',
			username: 'quanta-kt',
			url: 'https://github.com/quanta-kt',
			icon: 'icon-github',
			bg: 'bg-black'
		},
		{
			name: 'Discord',
			username: 'quanta.rs',
			url: 'https://discord.com/users/721012149933310029',
			bg: 'bg-[#404eed]',
			icon: 'icon-discord'
		},
		{
			name: 'LinkedIn',
			username: 'abhijeet-nkt',
			url: 'https://www.linkedin.com/in/abhijeet-kt/',
			bg: 'bg-[#0a66c2]',
			icon: 'icon-linkedin'
		},
		{
			name: 'e-mail',
			username: 'abhijeet.nkt@gmail.com',
			url: 'mailto:abhijeet.nkt@gmail.com',
			bg: 'bg-yellow-600',
			icon: 'icon-email'
		}
	];
</script>

<Navbar />

<div class="max-w-screen-md mx-auto flex flex-col">
	<!-- Hero -->
	<div class="w-full lg:mx-0 mx-6">
		<section id="home" class="flex lg:flex-row flex-col justify-between gap-14">
			<div class="flex flex-col justify-center gap-5">
				<p>Hi 👋 I am</p>
				<p class="text-6xl font-bold underline">Abhijeet Sonar</p>
				<div class="mt-3">
					<div class="relative">
						<p class="aaa1 font-bold text-xl absolute top-0 opacity-1">
							a <span class="underline">mobile</span> developer
						</p>
						<p class="aaa2 font-bold text-xl absolute top-0 opacity-0">
							a <span class="underline">web</span> developer
						</p>
						<p class="aaa3 font-bold text-xl absolute top-0 opacity-0">
							a <span class="underline">backend</span> developer
						</p>
						<p class="aaa4 font-bold text-xl absolute top-0 opacity-0">
							a <span class="underline">code</span> fanatic
						</p>
					</div>
				</div>
			</div>
		</section>

		<!-- Social -->
		<section id="socials" class="mt-20">
			<h2 class="text-3xl font-bold mb-4">Socials</h2>

			<div class="flex gap-4 flex-wrap">
				{#each socials as social}
					<a href={social.url} class={`${social.bg} flex p-2 gap-3`}>
						<div class={`${social.icon} p-2 w-10 h-10 bg-no-repeat bg-contain bg-center`} />

						<div class="text-white flex flex-col">
							<p class="text-xs">{social.name}</p>
							<p class="text-lg font-bold">{social.username}</p>
						</div>
					</a>
				{/each}
			</div>
		</section>

		<section id="projects"></section>

		<section id="blogs"></section>
	</div>
</div>

<style>
	.icon-github {
		background-image: url('$lib/assets/github-mark-white.png');
	}
	.icon-discord {
		background-image: url('$lib/assets/discord-mark-white.png');
	}
	.icon-linkedin {
		background-image: url('$lib/assets/linkedin-mark-white.png');
	}
	.icon-email {
		background-image: url('$lib/assets/email-mark-white.png');
	}

	.aaa1 {
		animation: switch-text 8s infinite;
	}
	.aaa2 {
		animation: switch-text 8s infinite 2s;
	}
	.aaa3 {
		animation: switch-text 8s infinite 4s;
	}
	.aaa4 {
		animation: switch-text 8s infinite 6s;
	}

	@keyframes switch-text {
		0% {
			transform: translatey(15px);
			opacity: 0;
		}
		20% {
			transform: translatey(0px);
			opacity: 1;
		}
		35% {
			transform: translatey(-15px);
			opacity: 0;
		}
		100% {
			opacity: 0;
		}
	}
</style>
