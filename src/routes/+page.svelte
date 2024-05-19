<script lang="ts">
	import Navbar from '$lib/components/Navbar.svelte';
</script>

<Navbar />

<!-- Hero -->
<div id="home" class="max-w-screen-md mx-auto flex">
	<div class="w-full flex lg:mx-0 mx-6 lg:flex-row flex-col justify-between gap-14">
		<div id="avatar" class="w-52 h-52 bg-no-repeat bg-cover" />

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
	</div>
</div>

<div id="socials"></div>

<div id="projects"></div>

<div id="blogs"></div>

<style>
	#avatar {
		background-image: url(https://vignette.wikia.nocookie.net/konosuba/images/7/7b/Aqua_Artwork_03.png/revision/latest?cb%5Cu003d20180608054657);
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
