<template>
  <div>
    <section-intro />

    <section-features />

    <section-get-started />

    <section-overview />

    <section-faq />
  </div>
</template>

<script>
import SectionFaq from '@/components/home/FAQ.vue'
import SectionIntro from '@/components/home/Intro.vue'
import SectionFeatures from '@/components/home/Features.vue'
import SectionOverview from '@/components/home/Overview.vue'
import SectionGetStarted from '@/components/home/GetStarted.vue'

export default {
  name: 'Home',

  components: {
    SectionFaq,
    SectionIntro,
    SectionFeatures,
    SectionOverview,
    SectionGetStarted
  }
}
</script>
