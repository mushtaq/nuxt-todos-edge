<script setup lang="ts">
// const host = useRequestURL().host
// let hosting = { url: 'https://pages.cloudflare.com', title: 'CloudFlare Pages' }
// if (host.includes('.netlify.app')) {
//   hosting = { url: 'https://www.netlify.com/products/#netlify-edge-functions', title: 'Netlify Edge Functions' }
// } else if (host.includes('.vercel.app')) {
//   hosting = { url: 'https://vercel.com/features/edge-functions', title: 'Vercel Edge Functions' }
// } else if (host.includes('.lagon.dev')) {
//   hosting = { url: 'https://lagon.app', title: 'Lagon' }
// } else if (host.includes('.deno.dev')) {
//   hosting = { url: 'https://deno.com/deploy', title: 'Deno Deploy' }
// }
// const isD1 = host.includes('nuxt-todos-edge.pages.dev')
// const { loggedIn } = useUserSession()
</script>

<template>
  <UCard>
    <template #header>
      <h3 class="text-lg font-semibold leading-6">
        Todo List
      </h3>
      <!-- <UButton
        v-if="!loggedIn"
        to="/api/auth/github"
        icon="i-simple-icons-github"
        label="Login with GitHub"
        color="black"
        external
      /> -->
      <UButton
        to="/todos"
        icon="i-heroicons-list-bullet"
        label="Go to Todos"
        color="black"
      />
    </template>
    <p class="font-medium">
      Welcome to Nuxt Todos App.
    </p>
    <p>
      A <a href="https://nuxt.com" target="_blank" class="text-primary-500" rel="noopener">Nuxt</a> demo hosted on <a href="https://portal.azure.com" target="_blank" rel="noopener" class="text-primary-500">Azure</a> with server-side rendering on the edge and using <NuxtLink
        href="https://turso.tech"
        target="_blank"
        rel="noopener"
        class="text-primary-500"
      >
        Turso database
      </NuxtLink>.
    </p>
    <hr class="dark:border-gray-700">
    <p class="text-sm text-gray-700 dark:text-gray-300 italic">
      Source code: https://github.com/mushtaq/nuxt-todos-edge <br>
      <br>
      Coped from: https://github.com/atinux/nuxt-todos-edge <br>
      (removed the integration code for Github OAuth)
    </p>
  </UCard>
</template>
