<template>
	<div>
		<header>
			<nuxt-link to="/">Home</nuxt-link>
			<nuxt-link to="/about">About</nuxt-link>
			<nuxt-link to="/contact">Contact</nuxt-link>
		</header>

		<Nuxt />

		<footer>
			&copy; 2022 - paulus-lestyo.my.id
		</footer>
	</div>
</template>

<style>
	body {
		font-family: sans-serif;
		margin: 15%;
	}
</style>