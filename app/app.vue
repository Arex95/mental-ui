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

const title = 'Solace - Mental Health & Wellness Miami'
const description = 'Compassionate psychiatric care and therapy in Miami. Discover a holistic, garden-inspired approach to mental well-being.'

useSeoMeta({
  title,
  description,
  ogTitle: title,
  ogDescription: description,
  ogImage: '/wellness.png',
  twitterImage: '/wellness.png',
  twitterCard: 'summary_large_image'
})
</script>

<template>
  <UApp>
    <UHeader class="border-b-0 bg-neutral-50/80 backdrop-blur-md sticky top-0 z-50">
      <template #left>
        <NuxtLink to="/" class="flex items-center gap-2 group">
          <div class="w-8 h-8 bg-primary-400 rounded-full flex items-center justify-center transition-transform group-hover:rotate-12">
            <UIcon name="i-lucide-sun" class="w-5 h-5 text-white" />
          </div>
          <span class="text-2xl font-serif font-bold text-neutral-900">Solace</span>
          <span class="text-[10px] font-bold tracking-[0.2em] uppercase text-primary-600 hidden sm:inline ml-1">Mental Health</span>
        </NuxtLink>
      </template>

      <template #center>
        <UHeaderMenu :links="[{
          label: 'Services',
          to: '#services'
        }, {
          label: 'Approach',
          to: '#philosophy'
        }, {
          label: 'Miami Oasis',
          to: '#about'
        }, {
          label: 'Contact',
          to: '#contact'
        }]" class="font-medium" />
      </template>

      <template #right>
        <UButton label="Book Visit" color="primary" variant="solid" class="rounded-full px-6 font-bold" />
      </template>
    </UHeader>

    <UMain>
      <NuxtPage />
    </UMain>

    <UFooter class="border-t-0 bg-neutral-100 py-16">
      <template #left>
        <div class="flex flex-col gap-4">
          <div class="flex items-center gap-2">
            <div class="w-6 h-6 bg-primary-400 rounded-full flex items-center justify-center">
              <UIcon name="i-lucide-sun" class="w-4 h-4 text-white" />
            </div>
            <span class="text-xl font-serif font-bold text-neutral-900">Solace</span>
          </div>
          <p class="text-sm text-neutral-500 max-w-xs leading-relaxed">
            Cultivating mental well-being through compassionate, evidence-based care in the heart of Florida.
          </p>
        </div>
      </template>

      <template #right>
        <div class="flex gap-4">
          <UButton to="https://instagram.com" target="_blank" icon="i-simple-icons-instagram" aria-label="Instagram"
            color="neutral" variant="ghost" class="hover:text-primary-600" />
          <UButton to="#" icon="i-simple-icons-linkedin" aria-label="LinkedIn"
            color="neutral" variant="ghost" class="hover:text-primary-600" />
        </div>
      </template>
    </UFooter>
  </UApp>
</template>
