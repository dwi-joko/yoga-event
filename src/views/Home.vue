<template>
  <div class="home">
    <Header></Header>
    <HeroImage></HeroImage>
    <BenefitSection></BenefitSection>
    <Blog></Blog>
    <Footer></Footer>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import HeroImage from '@/components/HeroImage.vue'
import BenefitSection from '@/components/BenefitSection.vue'
import Blog from '@/components/Blog.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'home',
  components: {
    Header,
    HeroImage,
    BenefitSection,
    Blog,
    Footer
  }
}
</script>
