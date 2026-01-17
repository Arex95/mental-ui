<template>
  <div class="selection:bg-primary-200">
    <!-- Hero Section -->
    <UPageHero 
      title="Nurturing Your Mind in the Heart of Miami"
      description="Experience psychiatric care that feels human. At Solace, we combine clinical excellence with a warm, organic approach to help your mental garden flourish."
      :links="[{
        label: 'Begin Your Journey',
        to: '#contact',
        size: 'xl',
        color: 'primary',
        class: 'rounded-full px-8'
      }, {
        label: 'Explore Our Approach',
        to: '#philosophy',
        size: 'xl',
        variant: 'link',
        color: 'neutral'
      }]" 
      align="left"
      class="py-24 sm:py-32"
    >
      <template #top>
        <span class="text-primary-600 font-serif italic text-lg mb-4 block">Welcome to Solace Mental Health</span>
      </template>

      <div class="relative group w-full max-w-xl">
        <div class="absolute inset-0 bg-primary-200/30 rounded-full blur-3xl -z-10 group-hover:bg-primary-300/40 transition-colors duration-700"></div>
        <div class="illustration-container card-organic shadow-2xl">
          <img src="/wellness.png" alt="Mental Wellness Illustration"
            class="w-full h-auto transform group-hover:scale-105 transition-transform duration-1000 p-8" />
        </div>
      </div>
    </UPageHero>

    <!-- Philosophy Section -->
    <UPageSection id="philosophy" class="bg-neutral-100 py-32 overflow-hidden relative" :ui="{ container: 'max-w-6xl' }">
      <div class="absolute top-0 right-0 w-64 h-64 bg-primary-100/50 rounded-full -mr-32 -mt-32 blur-3xl"></div>
      <div class="absolute bottom-0 left-0 w-96 h-96 bg-secondary-100/50 rounded-full -ml-48 -mb-48 blur-3xl"></div>
      
      <div class="relative z-10">
        <div class="text-center mb-16">
          <h2 class="text-primary-600 font-serif italic text-2xl mb-6">Our Philosophy</h2>
          <blockquote class="text-4xl md:text-5xl font-serif font-bold text-neutral-900 leading-tight max-w-4xl mx-auto">
            "Your mind is not a problem to be solved, but a garden to be nurtured."
          </blockquote>
        </div>
        
        <div class="grid grid-cols-1 md:grid-cols-2 gap-16 px-4">
          <div class="space-y-6">
            <p class="text-xl text-neutral-700 leading-relaxed font-light">
              We believe that mental health is a natural process of growth and balance. Located in the heart of Miami, we bring a warm, professional, and deeply human perspective to psychiatric care.
            </p>
          </div>
          <div class="space-y-6 border-l border-neutral-200 pl-8 hidden md:block">
            <p class="text-xl text-neutral-700 leading-relaxed font-light">
              Just as a garden needs the right environment to bloom, we provide the tools and support you need to find your inner calm amidst life's vibrant energy.
            </p>
          </div>
        </div>
      </div>
    </UPageSection>

    <!-- Services Section -->
    <UPageSection id="services" title="Cultivating Well-being"
      description="Explore our range of personalized services designed to support your unique journey with compassion and expertise."
      class="py-32"
    >
      <div class="grid grid-cols-1 md:grid-cols-3 gap-12 mt-16 w-full">
        <!-- Therapy Card -->
        <div class="flex flex-col group w-full">
          <div class="illustration-container card-organic mb-8 bg-primary-50 rounded-3xl aspect-square overflow-hidden">
            <img src="/therapy.png" alt="Psychotherapy" class="w-full h-full object-cover p-6 group-hover:scale-110 transition-transform duration-700" />
          </div>
          <h3 class="text-2xl font-serif font-bold text-neutral-900 mb-3">Individual Therapy</h3>
          <p class="text-neutral-600 text-lg leading-relaxed mb-6">
            Meaningful, evidence-based conversations focused on connection, understanding, and sustainable growth.
          </p>
          <UButton label="Learn More" variant="link" color="primary" class="p-0 text-lg w-fit" />
        </div>

        <!-- Evaluation Card -->
        <div class="flex flex-col group w-full">
          <div class="illustration-container card-organic mb-8 bg-secondary-50 rounded-3xl aspect-square overflow-hidden">
            <img src="/evaluation.png" alt="Evaluation" class="w-full h-full object-cover p-6 group-hover:scale-110 transition-transform duration-700" />
          </div>
          <h3 class="text-2xl font-serif font-bold text-neutral-900 mb-3">Psychiatric Evaluation</h3>
          <p class="text-neutral-600 text-lg leading-relaxed mb-6">
            Comprehensive assessments to understand your history and map out a personalized path to clarity.
          </p>
          <UButton label="Learn More" variant="link" color="primary" class="p-0 text-lg w-fit" />
        </div>

        <!-- Wellness Card -->
        <div class="flex flex-col group w-full">
          <div class="illustration-container card-organic mb-8 bg-neutral-100 rounded-3xl aspect-square overflow-hidden">
            <img src="/wellness.png" alt="Holistic Wellness" class="w-full h-full object-cover p-6 group-hover:scale-110 transition-transform duration-700" />
          </div>
          <h3 class="text-2xl font-serif font-bold text-neutral-900 mb-3">Holistic Wellness</h3>
          <p class="text-neutral-600 text-lg leading-relaxed mb-6">
            Integrating lifestyle, nutrition, and mindfulness to create a foundation for long-term mental resilience.
          </p>
          <UButton label="Learn More" variant="link" color="primary" class="p-0 text-lg w-fit" />
        </div>
      </div>
    </UPageSection>

    <!-- Miami Location Section -->
    <UPageSection id="about" class="bg-primary-50 py-32 overflow-hidden">
      <div class="grid grid-cols-1 lg:grid-cols-2 gap-20 items-center">
        <div class="relative order-2 lg:order-1">
          <div class="absolute inset-0 bg-white/40 backdrop-blur-sm rounded-[3rem] -z-10 transform -rotate-3 scale-105"></div>
          <img src="/hero.png" alt="Miami Serenity"
            class="w-full h-auto rounded-[3rem] shadow-2xl object-cover aspect-[4/5]" />
        </div>
        <div class="order-1 lg:order-2 px-4 lg:px-0">
          <h2 class="text-4xl md:text-5xl font-serif font-bold text-neutral-900 mb-8 leading-tight line-clamp-3">Finding Your Calm in the Neon City</h2>
          <p class="text-xl text-neutral-700 mb-8 leading-relaxed">
            Based in the serene heart of Miami, FL, we provide a sanctuary from the urban rush. Whether in-person or via telehealth, our space is designed to be your grounding force.
          </p>
          <div class="space-y-6 mb-10">
            <div class="flex items-center gap-4">
              <div class="w-12 h-12 bg-primary-100 rounded-full flex items-center justify-center text-primary-600">
                <UIcon name="i-lucide-map-pin" class="w-6 h-6" />
              </div>
              <div>
                <p class="font-bold text-neutral-900">Miami, Florida</p>
                <p class="text-neutral-600">Coral Gables & Virtual Visits</p>
              </div>
            </div>
            <div class="flex items-center gap-4">
              <div class="w-12 h-12 bg-primary-100 rounded-full flex items-center justify-center text-primary-600">
                <UIcon name="i-lucide-clock" class="w-6 h-6" />
              </div>
              <div>
                <p class="font-bold text-neutral-900">Flexible Scheduling</p>
                <p class="text-neutral-600">Morning & Evening Appointments</p>
              </div>
            </div>
          </div>
          <UButton label="Get Directions" variant="solid" color="neutral" size="xl" class="rounded-full px-8" />
        </div>
      </div>
    </UPageSection>

    <!-- CTA Section -->
    <UPageSection id="contact" class="py-32">
      <UPageCTA 
        title="Ready to Start Growing?"
        description="Book your initial consultation today. We're here to listen, support, and help you find your way forward."
        variant="solid" 
        color="primary" 
        class="rounded-[3rem] py-20 px-10 shadow-2xl"
        :links="[{
          label: 'Book Online',
          to: '#',
          icon: 'i-lucide-calendar',
          size: 'xl',
          class: 'bg-neutral-950 text-white hover:bg-neutral-800'
        }, {
          label: 'Call Us: (305) 555-0123',
          to: 'tel:3055550123',
          variant: 'link',
          color: 'neutral',
          size: 'xl'
        }]" 
      />
    </UPageSection>
    
    <!-- Footer -->
    <footer class="py-12 border-t border-neutral-200 text-center text-neutral-500 font-serif italic bg-neutral-50">
      <p>© 2026 Solace Mental Health. Helping Miami Bloom.</p>
    </footer>
  </div>
</template>
