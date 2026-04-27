<script>
import "../style.css";
export default {
  data() {
    return {
      showMenu: false,
      activeLink: '#home', // default active
      navbarItems: [
        { name: "Home", link: "#home" },
        { name: "Delivery", link: "#delivery" },
        { name: "About Us", link: "#about" },
        { name: "Prices", link: "#prices" },
        { name: "Contact", link: "#contact" },
      ],
      shadowHeader: false,
    };
  },
  methods:{
    handleShadow(){
      this.shadowHeader = window.scrollY >= 50
    }
  },

  mounted(){
      window.addEventListener('scroll',this.handleShadow)
    },
    beforeUnmount(){
      
      window.removeEventListener('scroll',this.handleShadow)
  }
};
</script>
 
<script setup>
import { ref, onMounted } from 'vue'
 
  localStorage.clear()

const isDark = ref(false)

// load theme + swiper
onMounted(() => {
  const saved = localStorage.getItem('theme')

  // ONLY apply dark if user explicitly selected it
  if (saved === 'dark') {
    document.body.classList.add('dark-theme')
    isDark.value = true
  } else {
    document.body.classList.remove('dark-theme') // force light mode
    isDark.value = false
    localStorage.setItem('theme', 'light') // set default
  }
 
})

// toggle theme
const toggleTheme = () => {
  isDark.value = !isDark.value

  document.body.classList.toggle('dark-theme')

  localStorage.setItem('theme', isDark.value ? 'dark' : 'light')
}
</script>



<style scoped>
/* Add Shadow Header */
.shadow-header{
    box-shadow: 0 2px 16px hsla(218,68%,18%,.1);
}

.active-link {
  color: var(--first-color);
  font-weight: 600;
}
</style>
  
  
<template>
  <header class="header" :class="{'shadow-header': shadowHeader}" id="header">
    <nav class="nav container">
      <a href="#" class="nav__logo" style="text-decoration: none">
        <i class="ri-stethoscope-line"></i> Medical
      </a>

      <div :class="['nav__menu', { 'show-menu': showMenu }]" id="nav-menu">
        <ul class="nav__list" style="list-style: none">
          <li v-for="(navItems,index) in navbarItems" :key="index">
            <a 
            :href="navItems.link"
            @click="activeLink = navItems.link; showMenu = false"
            :class="['nav__link', { 'active-link': activeLink === navItems.link }]">
            {{ navItems.name }}</a>
          </li>
          <div>{{ isLight }}</div>
        </ul>

        <!-- close btn -->
        <div
          class="nav__close"
          id="nav-close"
          @click.prevent="showMenu = false"
        >
          <i class="ri-close-large-line"></i>
        </div>
      </div>
      <div class="nav__btn">
        <!-- theme -->
          <i 
  :class="isDark ? 'ri-sun-fill' : 'ri-moon-fill'"
  class="nav__theme"
  @click="toggleTheme">
</i>

        <!-- Toggle btn -->
        <div
          class="nav__toggle"
          id="nav-toggle"
          @click="showMenu = true"
        >
          <i class="ri-menu-line"></i>
        </div>
      </div>
    </nav>
     
  </header>
</template>
