<template>
	<div class="mx-8 my-8">
		<header class="my-4 md:my-0 md:flex md:gap-2 md:justify-between">
			<div class="text-center p-2 my-8 md:my-0">
				<span class="soft-card p-4 text-center">🅿 Pauls</span>
			</div>
			<nav class="flex gap-2 md:gap-8 text-sm text-blue-400 justify-evenly">
				<nuxt-link class="soft-card px-4 py-2" to="/">Home</nuxt-link>
				<nuxt-link class="soft-card px-4 py-2" to="/about">About</nuxt-link>
				<nuxt-link class="soft-card px-4 py-2" to="/blog">Blog</nuxt-link>
				<nuxt-link class="soft-card px-4 py-2" to="/contact">Contact</nuxt-link>
			</nav>
		</header>

		<div class="my-10 soft-card min-h-[300px] p-3 text-sm">
			<Nuxt />
		</div>

		<footer class="my-4 mx-auto text-center soft-card px-4 py-2 text-sm md:text-base">
			&copy; 2022 - paulus-lestyo.my.id
		</footer>
	</div>
</template>