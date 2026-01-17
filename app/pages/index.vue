<template>
  <div class="selection:bg-primary-200">
    <!-- Hero Section -->
    <div class="relative overflow-hidden bg-neutral-50 pt-16 pb-32">
      <UContainer>
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
          <div class="max-w-2xl">
            <span class="text-primary-600 font-serif italic text-lg mb-4 block">Welcome to Solace Mental Health</span>
            <h1 class="text-5xl md:text-7xl font-serif font-bold text-neutral-900 leading-tight mb-8">
              Nurturing Your Mind in the Heart of Miami
            </h1>
            <p class="text-xl text-neutral-600 mb-10 leading-relaxed max-w-lg">
              Experience psychiatric care that feels human. At Solace, we combine clinical excellence with a warm, organic approach to help your mental garden flourish.
            </p>
            <div class="flex flex-wrap gap-4">
              <UButton label="Begin Your Journey" to="#contact" size="xl" color="primary" class="rounded-full px-8 font-bold" />
              <UButton label="Explore Our Approach" to="#philosophy" size="xl" variant="link" color="neutral" class="font-medium" />
            </div>
          </div>
          <div class="relative group">
            <div class="absolute inset-0 bg-primary-200/30 rounded-full blur-3xl -z-10 group-hover:bg-primary-300/40 transition-colors duration-700"></div>
            <div class="illustration-container card-organic shadow-2xl bg-white/50 backdrop-blur-sm p-4">
              <img src="/wellness.png" alt="Mental Wellness Illustration"
                class="w-full h-auto transform group-hover:scale-105 transition-transform duration-1000" />
            </div>
          </div>
        </div>
      </UContainer>
    </div>

    <!-- Philosophy Section -->
    <div id="philosophy" class="bg-neutral-100 py-32 overflow-hidden relative">
      <div class="absolute top-0 right-0 w-64 h-64 bg-primary-100/50 rounded-full -mr-32 -mt-32 blur-3xl opacity-50"></div>
      <div class="absolute bottom-0 left-0 w-96 h-96 bg-secondary-100/50 rounded-full -ml-48 -mb-48 blur-3xl opacity-50"></div>
      
      <UContainer class="relative z-10">
        <div class="text-center mb-20">
          <h2 class="text-primary-600 font-serif italic text-2xl mb-6">Our Philosophy</h2>
          <blockquote class="text-4xl md:text-6xl font-serif font-bold text-neutral-900 leading-tight max-w-5xl mx-auto">
            "Your mind is not a problem to be solved, but a garden to be nurtured."
          </blockquote>
        </div>
        
        <div class="grid grid-cols-1 md:grid-cols-2 gap-20">
          <p class="text-2xl text-neutral-700 leading-relaxed font-light">
            We believe that mental health is a natural process of growth and balance. Located in the heart of Miami, we bring a warm, professional, and deeply human perspective to psychiatric care.
          </p>
          <p class="text-2xl text-neutral-700 leading-relaxed font-light md:border-l md:border-neutral-300 md:pl-12">
            Just as a garden needs the right environment to bloom, we provide the tools and support you need to find your inner calm amidst life's vibrant energy.
          </p>
        </div>
      </UContainer>
    </div>

    <!-- Services Section -->
    <div id="services" class="py-32 bg-white">
      <UContainer>
        <div class="max-w-3xl mb-16">
          <h2 class="text-4xl font-serif font-bold text-neutral-900 mb-6 font-serif italic">Cultivating Well-being</h2>
          <p class="text-xl text-neutral-600 leading-relaxed">
            Explore our range of personalized services designed to support your unique journey with compassion and expertise.
          </p>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-12">
          <!-- Therapy Card -->
          <div class="flex flex-col group py-4">
            <div class="illustration-container card-organic mb-8 bg-primary-50 rounded-[2rem] overflow-hidden aspect-square flex items-center justify-center p-8">
              <img src="/therapy.png" alt="Psychotherapy" class="w-full h-full object-contain group-hover:scale-110 transition-transform duration-700" />
            </div>
            <h3 class="text-2xl font-serif font-bold text-neutral-900 mb-4">Individual Therapy</h3>
            <p class="text-neutral-600 text-lg leading-relaxed mb-6">
              Meaningful, evidence-based conversations focused on connection, understanding, and sustainable growth.
            </p>
            <UButton label="Discover More" variant="link" color="primary" class="p-0 text-lg w-fit font-bold" />
          </div>

          <!-- Evaluation Card -->
          <div class="flex flex-col group py-4">
            <div class="illustration-container card-organic mb-8 bg-secondary-50 rounded-[2rem] overflow-hidden aspect-square flex items-center justify-center p-8">
              <img src="/evaluation.png" alt="Evaluation" class="w-full h-full object-contain group-hover:scale-110 transition-transform duration-700" />
            </div>
            <h3 class="text-2xl font-serif font-bold text-neutral-900 mb-4">Psychiatric Evaluation</h3>
            <p class="text-neutral-600 text-lg leading-relaxed mb-6">
              Comprehensive assessments to understand your history and map out a personalized path to clarity.
            </p>
            <UButton label="Discover More" variant="link" color="primary" class="p-0 text-lg w-fit font-bold" />
          </div>

          <!-- Wellness Card -->
          <div class="flex flex-col group py-4">
            <div class="illustration-container card-organic mb-8 bg-neutral-100 rounded-[2rem] overflow-hidden aspect-square flex items-center justify-center p-8">
              <img src="/wellness.png" alt="Holistic Wellness" class="w-full h-full object-contain group-hover:scale-110 transition-transform duration-700" />
            </div>
            <h3 class="text-2xl font-serif font-bold text-neutral-900 mb-4">Holistic Wellness</h3>
            <p class="text-neutral-600 text-lg leading-relaxed mb-6">
              Integrating lifestyle, nutrition, and mindfulness to create a foundation for long-term mental resilience.
            </p>
            <UButton label="Discover More" variant="link" color="primary" class="p-0 text-lg w-fit font-bold" />
          </div>
        </div>
      </UContainer>
    </div>

    <!-- Miami Location Section -->
    <div id="about" class="bg-primary-50 py-32 overflow-hidden">
      <UContainer>
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-20 items-center">
          <div class="relative order-2 lg:order-1">
            <div class="absolute inset-0 bg-white/40 backdrop-blur-sm rounded-[3rem] -z-10 transform -rotate-3 scale-105"></div>
            <img src="/hero.png" alt="Miami Serenity"
              class="w-full h-auto rounded-[3rem] shadow-2xl object-cover aspect-[4/5]" />
          </div>
          <div class="order-1 lg:order-2">
            <h2 class="text-4xl md:text-6xl font-serif font-bold text-neutral-900 mb-8 leading-tight">Finding Your Calm in the Neon City</h2>
            <p class="text-2xl text-neutral-700 mb-10 leading-relaxed font-light">
              Based in the serene heart of Miami, FL, we provide a sanctuary from the urban rush. Whether in-person or via telehealth, our space is designed to be your grounding force.
            </p>
            <div class="space-y-8 mb-12">
              <div class="flex items-center gap-6">
                <div class="w-14 h-14 bg-white rounded-2xl shadow-sm flex items-center justify-center text-primary-600">
                  <UIcon name="i-lucide-map-pin" class="w-7 h-7" />
                </div>
                <div>
                  <p class="text-xl font-bold text-neutral-900">Miami, Florida</p>
                  <p class="text-lg text-neutral-600">Coral Gables & Virtual Visits</p>
                </div>
              </div>
              <div class="flex items-center gap-6">
                <div class="w-14 h-14 bg-white rounded-2xl shadow-sm flex items-center justify-center text-primary-600">
                  <UIcon name="i-lucide-clock" class="w-7 h-7" />
                </div>
                <div>
                  <p class="text-xl font-bold text-neutral-900">Flexible Scheduling</p>
                  <p class="text-lg text-neutral-600">Morning & Evening Appointments</p>
                </div>
              </div>
            </div>
            <UButton label="Get Directions" variant="solid" color="neutral" size="xl" class="rounded-full px-10 font-bold" />
          </div>
        </div>
      </UContainer>
    </div>

    <!-- CTA Section -->
    <div id="contact" class="py-32">
      <UContainer>
        <UPageCTA 
          title="Ready to Start Growing?"
          description="Book your initial consultation today. We're here to listen, support, and help you find your way forward."
          variant="solid" 
          color="primary" 
          class="rounded-[3rem] py-24 px-12 shadow-2xl relative overflow-hidden"
          :links="[{
            label: 'Book Online',
            to: '#',
            icon: 'i-lucide-calendar',
            size: 'xl',
            class: 'bg-neutral-950 text-white hover:bg-neutral-800 rounded-full px-8'
          }, {
            label: 'Call Us: (305) 555-0123',
            to: 'tel:3055550123',
            variant: 'link',
            color: 'neutral',
            size: 'xl',
            class: 'hover:text-neutral-900'
          }]" 
        >
          <template #top>
            <div class="absolute top-0 right-0 w-64 h-64 bg-white/20 rounded-full -mr-32 -mt-32 blur-3xl"></div>
          </template>
        </UPageCTA>
      </UContainer>
    </div>
    
    <!-- Footer -->
    <footer class="py-16 border-t border-neutral-200 text-center bg-neutral-100">
      <UContainer>
        <div class="mb-8">
          <span class="text-3xl font-serif font-bold text-neutral-900">Solace</span>
        </div>
        <p class="text-neutral-500 font-serif italic text-lg mb-4">Helping Miami Bloom.</p>
        <p class="text-neutral-400 text-sm">© {{ new Date().getFullYear() }} Solace Mental Health. All rights reserved.</p>
      </UContainer>
    </footer>
  </div>
</template>
