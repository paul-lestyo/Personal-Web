<template>
  <div class="">
    <header class="w-full h-16 bg-green-500">
      <nav class="flex items-center justify-center w-full h-full text-center text-black">
        <ul class="list-none flex gap-4 justify-center">
          <li class="inline">
            <NuxtLink to="/">Home</NuxtLink>
          </li>
          <li class="inline">
            <NuxtLink to="/about">About</NuxtLink>
          </li>
          <li class="inline">
            <NuxtLink to="/contact">Contact</NuxtLink>
          </li>
        </ul>
      </nav>
    </header>
    <main class="flex-grow w-full h-full p-4 mx-auto max-w-7xl">
      <slot />
    </main>
    <footer class="flex items-center justify-center w-full h-16 text-black">
      <p class="text-gray-700">My Nuxt App &copy; {{ new Date().getFullYear() }}</p>
    </footer>
  </div>
</template>