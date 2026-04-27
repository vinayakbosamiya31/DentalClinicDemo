
<template>
    <section class="gallery section">
        <div class="gallery__container container grid">
            <!-- Image -->
             <div class="gallery__image">
                <img src="../assets/g1.png" alt="Image" class="gallery_img">
             </div>
             <div class="gallery__image">
                <img src="../assets/g2.png" alt="Image" class="gallery_img">
             </div>
             <div class="gallery__image">
                <img src="../assets/g3.png" alt="Image" class="gallery_img">
             </div>
             <div class="gallery__image">
                <img src="../assets/g4.png" alt="Image" class="gallery_img">
             </div>
             <div class="gallery__image">
                <img src="../assets/g5.png" alt="Image" class="gallery_img">
             </div>
        </div>
    </section>

    <!-- contact section -->
     <section class="contact section" id="contact">
        <div class="content__container container grid">
            <div class="contact__data">
                <h2 class="section__title">
                    Contact Me <br>
                    <span>On All Platforms</span>
                </h2>

                <p class="contact__description">
                    Convert me on all my Lorem ipsum dolor sit amet 
                    labore delectus similique eveniet illum debitis? 
                </p>

                <div class="contact__info">
                    <div>
                        <div class="contact__icon">
                            <i class="ri-question-answer-fill"></i>
                        </div>
                        <h3 class="contact__subtitle">Write to me</h3>
                        <div class="contact__social">
                            <a href="" class="contact__social-link" target="blank">
                                <i class="ri-messenger-fill"></i>
                            </a>
                            <a href="" class="contact__social-link" target="blank">
                                <i class="ri-whatsapp-fill"></i>
                            </a>
                            <a href="" class="contact__social-link" target="blank">
                                <i class="ri-telegram-2-fill"></i>
                            </a>
                            <a href="" class="contact__social-link" target="blank">
                                <i class="ri-mail-fill"></i>
                            </a>
                        </div>
                    </div>
                     
                    <div>
                        <div class="contact__icon">
                            <i class="ri-hospital-fill"></i>
                        </div>
                        <h3 class="contact__subtitle">Location</h3>
                        <address class="contact__address">
                            abc <br>
                            123
                        </address>
                    </div>
                    
                    <div>
                        <div class="contact__icon">
                            <i class="ri-time-fill"></i>
                        </div>
                        <h3 class="contact__subtitle">Attention</h3>
                        <address class="contact__address">
                            Monday - Saturday
                            10am - 8pm
                        </address>
                    </div>

                    <div>
                        <div class="contact__icon">
                            <i class="ri-smartphone-fill"></i>
                        </div>
                        <h3 class="contact__subtitle">Phone number</h3>
                        <address class="contact__address">
                            +91 12321230
                        </address>
                    </div>

                </div>
            </div>
            <div class="content__map">
                <iframe
                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3297.4193642115065!2d70.78562241023249!3d22.294214743032406!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3959ca19b942ac15%3A0xc9b0cf2d987d43b6!2sRotary%20International%20Dolls%20Museum!5e1!3m2!1sen!2sin!4v1777096897737!5m2!1sen!2sin"
                width="100%"
                height="450"
                style="border:0;"
                loading="lazy"></iframe>
            </div>
        </div>
    </section>
</template>