<script lang="ts">
	const navItems = [
		{
			title: 'Home',
			href: '#home',
			active: true
		},
		{
			title: 'Projects',
			href: '#projects'
		},
		{
			title: 'Blog',
			href: 'https://blog.qunatablob.xyz/'
		}
	];
</script>

<div class="flex justify-center gap-8 py-8 mx-auto">
	{#each navItems as item}
		<a
			class={`${item.active ? 'font-bold underline' : ''}
			text-2xl underline-offset-4 decoration-4`}
			href={item.href}>{item.title}</a
		>
	{/each}
</div>
