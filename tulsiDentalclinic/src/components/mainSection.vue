<template>
  <main class="main">
    <section class="home-section" id="home">
      <div class="home__container container grid">
        <div class="home__data">
          <h1 class="home__title">
            <span>Get Quick</span><br />
            Medical Service
          </h1>

          <p class="home__description">
            Get your medical services from a certified doctor and health
            professional.
          </p>

          <a href="#delivery" class="button">Get Started</a>
        </div>
        <div class="home__content grid">
          <div class="home__info">
            <div>
              <h2 class="home__name">Ramesh janni</h2>
              <h3 class="home__profession">Dentist Specialist</h3>

              <div class="home__icons">
                <div class="home__box">
                  <i class="ri-medicine-bottle-fill"></i>
                </div>
                <div class="home__box">
                  <i class="ri-24-hours-fill"></i>
                </div>
              </div>
            </div>
            <a href="#contact" class="home__button button-dark"
              ><i class="ri-arrow-right-s-line"></i>
              <span class="text"> Contact</span>
            </a>
          </div>
          <div class="home__image">
            <img
              src="../assets/doctor.png"
              alt="doctorImage"
              class="home__img"
            />
          </div>
        </div>
      </div>
    </section>

    <!-- Delivery -->
    <section class="delivery section" id="delivery">
      <div class="delivery__container container grid">
        <div class="delivery__data">
          <h2 class="section__title">
            Vaccine Injections <br />
            <span>Delivery Service</span>
          </h2>

          <p class="delivery__description">
            We provide door-to-door vaccine and injection delivery services,
            available to all segments throughout the city.
          </p>

          <div class="delivery__info">
            <div>
              <div class="delivery__icon">
                <i class="ri-home-5-fill"></i>
              </div>
              <h3 class="delivery__subtitle">Home Service</h3>
              <p>Fast Home Vaccination Service.</p>
            </div>

            <div>
              <div class="delivery__icon">
                <i class="ri-timer-fill"></i>
              </div>
              <h3 class="delivery__subtitle">1 Hour Service</h3>
              <p>Super Easy And Quick Service for Patients.</p>
            </div>

            <div>
              <div class="delivery__icon">
                <i class="ri-syringe-fill"></i>
              </div>
              <h3 class="delivery__subtitle">Better Quality</h3>
              <p>The Best Medicines for Health.</p>
            </div>
          </div>
        </div>
        <div class="delivery__content">
          <h3 class="delivery__title">
            Request <br />
            Vaccination
          </h3>
          <p class="delivery__patients"><span>324</span> Patients.</p>

          <div class="delivery__image">
            <img
              src="../assets/vaccination.png"
              alt="image"
              class="delivery__img"
            />
          </div>

          <a href="#content" class="button-dark">
            Request
            <i class="ri-arrow-right-s-line"></i>
          </a>
        </div>
      </div>
    </section>

    <!-- About section -->
    <section class="about section" id="about">
      <div class="about__container container grid">
        <div class="about__data">
          <div>
            <h2 class="section__title">
              <span>We Have Certified</span>
              <br />
              Medical Service
            </h2>

            <p class="about__description">
              Don't Worry, We have Certified medical services,so you can receive
              medical consultations in any specialty.
            </p>
          </div>

          <div class="about__info">
            <div class="about__stat">
              <h3 class="about__number">256</h3>
              <p class="about__details">
                Healthy <br />
                Patients
              </p>
            </div>

            <div class="about__stat">
              <h3 class="about__number">16</h3>
              <p class="about__details">
                Hospital <br />
                Care
              </p>
            </div>

            <div class="about__stat">
              <h3 class="about__number">8</h3>
              <p class="about__details">
                Years Of <br />
                Experience
              </p>
            </div>
          </div>

          <a href="#contact" class="about__button">
            Contact Me
            <i class="ri-arrow-right-s-line"></i>
          </a>
        </div>
        <img src="../assets/about.png" alt="about Image" class="about__img" />
      </div>
    </section>

    <!-- prices section -->
    <section class="prices section" id="prices">
      <div class="prices__container container grid">
        <div class="prices__data">
          <h2 class="section__title">
            <span>Affordable Prices To</span>
            <br>Check your Health
          </h2>

          <p class="prices__description">
            Get the best prices,make inquires , checkups, and 
            visit your home. Schedule Your consultations now.
          </p>
        </div>

        <div class="prices__content">
          <div class="prices__box">
            <p class="prices__details">All medical services <br> In your Hand</p>
          </div>

          <div class="prices__swiper swiper">
            <div class="swiper-wrapper">
              <article class="prices__card swiper-slide">
                <div class="prices__heading">
                  <h2 class="prices__number">₹10</h2>
                  <h3 class="prices__title">Health consultations</h3>
                </div>

                <ul class="prices__list">
                  <li class="prices__item">
                    <i class="ri-checkbox-fill"></i>
                    <span>consultations About your health.</span>
                  </li>

                  <li class="prices__item">
                    <i class="ri-checkbox-fill"></i>
                    <span>Ask Any Questions About your health.</span>
                  </li>

                  <li class="prices__item">
                    <i class="ri-checkbox-fill"></i>
                    <span>Take Your Time Without Limit.</span>
                  </li>
                </ul>
              </article>
               
              <article class="prices__card swiper-slide">
                <div class="prices__heading">
                  <h2 class="prices__number">₹20</h2>
                  <h3 class="prices__title">Delivery Services</h3>
                </div>

                <ul class="prices__list">
                  <li class="prices__item">
                    <i class="ri-checkbox-fill"></i>
                    <span>We Offer Delivery Services.</span>
                  </li>
                  <li class="prices__item">
                    <i class="ri-checkbox-fill"></i>
                    <span>We come to your home for service.</span>
                  </li>
                  <li class="prices__item">
                    <i class="ri-checkbox-fill"></i>
                    <span>Available 24 Hours a day.</span>
                  </li>
                </ul>
              </article>
               
              <article class="prices__card swiper-slide">
                <div class="prices__heading">
                  <h2 class="prices__number">₹30</h2>
                  <h3 class="prices__title">Delivery Services</h3>
                </div>

                <ul class="prices__list">
                  <li class="prices__item">
                    <i class="ri-checkbox-fill"></i>
                    <span>We Offer Delivery Services.</span>
                  </li>
                  <li class="prices__item">
                    <i class="ri-checkbox-fill"></i>
                    <span>We come to your home for service.</span>
                  </li>
                  <li class="prices__item">
                    <i class="ri-checkbox-fill"></i>
                    <span>Available 24 Hours a day.</span>
                  </li>
                </ul>
              </article>
            </div>
            <!-- Pagination -->
            <div class="swiper-pagination" ></div>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>
<script>
import Swiper from 'swiper'
import 'swiper/css'
import 'swiper/css/pagination'

import { Pagination, Autoplay } from 'swiper/modules'

export default {
  mounted() {
    new Swiper('.prices__swiper', {
      modules: [Pagination, Autoplay],

      loop: true,
      grabCursor: true,
      spaceBetween: 24,

      pagination: {
        el: '.swiper-pagination',
        clickable: true,
      },

      // autoplay: {
      //   delay: 3000,
      //   disableOnInteraction: false,
      // },
    })
  }

  
}
</script>

<style>
:root {
  --bullet-color: rgb(19, 19, 19);
}

body.dark-theme {
  --bullet-color: white;
}

.swiper-pagination-bullet {
  background-color: var(--bullet-color);
}</style>