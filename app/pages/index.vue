<template>
  <div>
    <UPageHero title="Mindful Healing in the Heart of Miami"
      description="Specialized psychiatric care and therapy tailored to your unique journey. At Solace, we combine clinical expertise with a compassionate, holistic approach to help you find your inner balance."
      :links="[{
        label: 'Schedule a Consultation',
        to: '#contact',
        size: 'xl',
        color: 'primary'
      }, {
        label: 'Our Services',
        to: '#services',
        size: 'xl',
        variant: 'link',
        color: 'neutral'
      }]" align="left">
      <template #top>
        <span class="text-primary font-medium tracking-wide uppercase text-sm mb-4 block">Welcome to Solace Mental
          Health</span>
      </template>

      <div class="relative w-full aspect-square max-w-lg mx-auto lg:mr-0">
        <div class="absolute inset-0 bg-primary-100/50 rounded-full blur-3xl -z-10 animate-pulse"></div>
        <img src="/hero.png" alt="Meditation at Miami Beach"
          class="w-full h-auto rounded-2xl shadow-2xl transform hover:scale-[1.02] transition-transform duration-500" />
      </div>
    </UPageHero>

    <UPageSection class="bg-cream py-24">
      <div class="max-w-3xl mx-auto text-center">
        <blockquote class="text-3xl font-serif italic text-neutral-800 leading-relaxed">
          "Your mind is like the ocean; sometimes turbulent, sometimes calm, but always deep and full of life. We help
          you
          navigate the waves."
        </blockquote>
        <p class="mt-8 text-lg text-soft">
          Solace Mental Health provides a sanctuary for those seeking clarity and growth amidst the vibrant energy of
          Miami.
        </p>
      </div>
    </UPageSection>

    <UPageSection id="services" title="Personalized Care for Your Mind"
      description="We offer a range of services designed to support your mental well-being at every stage of life.">
      <template #features>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
          <UPageCard title="Psychiatric Evaluation"
            description="Comprehensive clinical assessments to understand your unique needs and develop a personalized treatment plan.">
            <template #icon>
              <div class="p-3 bg-secondary-100 rounded-xl mb-4">
                <UIcon name="i-lucide-brain" class="w-8 h-8 text-secondary-600" />
              </div>
            </template>
          </UPageCard>

          <UPageCard title="Psychotherapy"
            description="Engaging, evidence-based therapy sessions focused on cognitive behavioral techniques and mindfulness.">
            <template #icon>
              <div class="p-3 bg-primary-100 rounded-xl mb-4">
                <UIcon name="i-lucide-messages-square" class="w-8 h-8 text-primary-600" />
              </div>
            </template>
          </UPageCard>

          <UPageCard title="Medication Management"
            description="Expert guidance and ongoing monitoring of psychiatric medications to ensure safety and effectiveness.">
            <template #icon>
              <div class="p-3 bg-neutral-100 rounded-xl mb-4">
                <UIcon name="i-lucide-pill" class="w-8 h-8 text-neutral-600" />
              </div>
            </template>
          </UPageCard>

          <UPageCard title="Holistic Wellness"
            description="Integrating nutritional guidance, sleep hygiene, and stress management into your mental health journey.">
            <template #icon>
              <div class="p-3 bg-secondary-100 rounded-xl mb-4">
                <UIcon name="i-lucide-sun" class="w-8 h-8 text-secondary-600" />
              </div>
            </template>
          </UPageCard>
        </div>
      </template>
    </UPageSection>

    <UPageSection id="about" class="bg-cream overflow-hidden">
      <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-center">
        <div>
          <h2 class="text-4xl font-serif font-bold text-neutral-900 mb-6">A Local Approach to Global Well-being</h2>
          <p class="text-lg text-neutral-600 mb-6">
            Located in the serene surroundings of Coral Gables, Solace Mental Health serves the greater Miami community
            with
            both in-person and tele-health visits.
          </p>
          <p class="text-lg text-neutral-600 mb-8">
            We understand the unique stressors of Miami life—from the high-paced urban environment to the search for
            balance. Our team is here to provide a grounded, professional, and warm space for your healing.
          </p>
          <UButton label="Learn More About Our Team" variant="outline" color="neutral" size="lg" />
        </div>
        <div class="relative">
          <div class="absolute -top-12 -right-12 w-64 h-64 bg-secondary-200/40 rounded-full blur-3xl -z-10"></div>
          <img src="/services.png" alt="Solace Mental Health Services Icons"
            class="w-full h-auto rounded-3xl shadow-xl bg-white p-8" />
        </div>
      </div>
    </UPageSection>

    <UPageSection id="contact">
      <UPageCTA title="Start Your Journey Today"
        description="Ready to take the first step towards a brighter, more balanced future? Book your initial consultation online or give us a call."
        variant="solid" color="primary" :links="[{
          label: 'Book Online',
          to: '#',
          icon: 'i-lucide-calendar',
          size: 'xl'
        }, {
          label: 'Call (305) 555-0123',
          to: 'tel:3055550123',
          variant: 'link',
          color: 'neutral',
          size: 'xl'
        }]" />
    </UPageSection>
  </div>
</template>
