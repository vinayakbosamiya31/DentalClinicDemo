<script setup>
import { ref, onMounted, onUnmounted } from "vue";

const linksNames = ref([
  { name: "Home", link: "#home" },
  { name: "About Us", link: "#about" },
  { name: "Prices", link: "#prices" },
]);
const icons = ref([
  "ri-facebook-box-fill",
  "ri-instagram-fill",
  "ri-twitter-x-fill",
  "ri-whatsapp-fill",
]);

const scrollUp = () => {
  const el = document.getElementById("scroll-up");

  if (window.scrollY >= 350) {
    el.classList.add("show-scroll");
  } else {
    el.classList.remove("show-scroll");
  }
};

onMounted(() => {
  window.addEventListener("scroll", scrollUp);
});

onUnmounted(() => {
  window.removeEventListener("scroll", scrollUp);
});


// function
const scrollActive = () => {
  const sections = document.querySelectorAll('section[id]')
  const scrollY = window.scrollY

  sections.forEach((current) => {
    const sectionHeight = current.offsetHeight
    const sectionTop = current.offsetTop - 58
    const sectionId = current.getAttribute('id')

    const link = document.querySelector(`.nav__menu a[href*="${sectionId}"]`)

    if (!link) return  // safety

    if (scrollY > sectionTop && scrollY <= sectionTop + sectionHeight) {
      link.classList.add('active-link')
    } else {
      link.classList.remove('active-link')
    }
  })
}

// lifecycle
onMounted(() => {
  window.addEventListener('scroll', scrollActive)
})

onUnmounted(() => {
  window.removeEventListener('scroll', scrollActive)
})
</script>
<template>
  <footer class="footer">
    <div class="footer__container container grid">
      <a href="#" class="footer__logo">
        <i class="ri-stethoscope-line"></i> Medical
      </a>
      <div class="footer__links">
        <a
          v-for="linksName in linksNames"
          :href="linksName.link"
          class="footer__link"
          >{{ linksName.name }}</a
        >
      </div>
      <div class="footer__social">
        <a
          href=""
          target="_blank"
          class="footer__social-link"
          v-for="i in icons"
        >
          <i :class="i"></i>
        </a>
      </div>
    </div>

    <span class="footer__copy"> &#169; All Rights Reserved By VINAY BOSAMIYA. </span>
  </footer>

  <a href="#" class="scrollup" id="scroll-up">
    <i class="ri-arrow-up-fill"></i>
  </a>
</template>
<script setup></script>
