<script setup>
useHead({
  meta: [
    { name: 'viewport', content: 'width=device-width, initial-scale=1' }
  ],
  link: [
    { rel: 'icon', href: '/favicon.ico' },
    { rel: 'preconnect', href: 'https://fonts.googleapis.com' },
    { rel: 'preconnect', href: 'https://fonts.gstatic.com', crossorigin: '' },
    { rel: 'stylesheet', href: 'https://fonts.googleapis.com/css2?family=Lora:ital,wght@0,400..700;1,400..700&family=Outfit:wght@100..900&display=swap' }
  ],
  htmlAttrs: {
    lang: 'en'
  }
})

const title = 'Solace Mental Health Miami | Psychiatric Care & Therapy'
const description = 'Compassionate, evidence-based psychiatric care and therapy in Miami. Discover a holistic approach to mental well-being with our expert team.'

useSeoMeta({
  title,
  description,
  ogTitle: title,
  ogDescription: description,
  ogImage: '/hero-bg.png',
  twitterImage: '/hero-bg.png',
  twitterCard: 'summary_large_image'
})
</script>

<template>
  <UApp>
    <UHeader>
      <template #left>
        <NuxtLink to="/" class="flex items-center gap-2">
          <span class="text-xl font-serif font-bold text-primary">Solace</span>
          <span class="text-sm font-light tracking-widest uppercase hidden sm:inline">Mental Health</span>
        </NuxtLink>
      </template>

      <template #center>
        <UHeaderMenu :links="[{
          label: 'Services',
          to: '#services'
        }, {
          label: 'About',
          to: '#about'
        }, {
          label: 'FAQ',
          to: '#faq'
        }, {
          label: 'Contact',
          to: '#contact'
        }]" />
      </template>

      <template #right>
        <UColorModeButton />

        <UButton label="Book Now" color="primary" variant="solid" class="hidden sm:flex" />
      </template>
    </UHeader>

    <UMain>
      <NuxtPage />
    </UMain>

    <UFooter>
      <template #left>
        <p class="text-sm text-muted">
          Solace Mental Health Miami • © {{ new Date().getFullYear() }}
        </p>
      </template>

      <template #right>
        <UButton to="https://instagram.com" target="_blank" icon="i-simple-icons-instagram" aria-label="Instagram"
          color="neutral" variant="ghost" />
      </template>
    </UFooter>
  </UApp>
</template>
