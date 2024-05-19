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
			<p class="">A motivated software developer</p>
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
</style>
