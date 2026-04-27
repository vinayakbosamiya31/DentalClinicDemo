<script>
 
import HeaderSection from './components/HeaderSection.vue'
import mainSection from './components/mainSection.vue'
import gallerySection from './components/gallarySection.vue';
import Footer from './components/footer.vue';

export default{
components:{
    HeaderSection,
    mainSection,
    gallerySection,
    Footer
  }, 
}

</script>

<script setup>
import { onMounted } from 'vue'
import ScrollReveal from 'scrollreveal'

onMounted(() => {
  const sr = ScrollReveal({
    origin: 'top', //comes from top ⬇️
    distance: '100px', //Element starts 60px above Then moves down to its original place // for example if 100px to elements is go to first below at 100px and element come to that real position
    duration: 1000,
    reset: true,        // ❌ no hiding
    viewFactor: 0.2,
  })
   sr.reveal('.home__content', { origin: 'bottom' })
  sr.reveal('.home__info', { origin: 'bottom', delay: 800 })
  sr.reveal('.home__data', { delay: 1400 })
  sr.reveal('.home__button', { origin: 'left', delay: 1800 })

  sr.reveal('.delivery__data', { origin: 'right', })
  sr.reveal('.delivery__content', { origin: 'left', delay:600 })
  sr.reveal('.delivery__img', { delay:1200 })

  sr.reveal('.about__data', {origin:'bottom' })
  sr.reveal('.about__img', {delay:120 })
  
  sr.reveal('.prices__box')
  sr.reveal('.prices__swiper', {delay:600 })

  sr.reveal('.contact__data', {
  origin: 'left',
  distance: '100px',
  duration: 1000,
  reset: false,
})

sr.reveal('.content__map', {
  origin: 'right',
  distance: '100px',
  duration: 1000,
  reset: false,
})
  
  sr.reveal('.gallery__image', {interval:100 })
  
  sr.reveal('.footer__container', {
  origin: 'right',
  distance: '100px',
  duration: 1000,
  reset: false,
})
})
</script>

<template>
  
  <HeaderSection/>
  <mainSection/>
  <gallerySection/>
  <Footer />

</template>


