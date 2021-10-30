<template>
  <div class="container mx-auto px-7 mb-20">
    <nav class="navbar flex justify-between items-center mb-5">
        <div class="py-2 navbar__logo">
            <a href="">
                <img src="~/assets/img/logo.png" alt="logo elemes.id">
            </a>
        </div>

        <!-- navigation -->
        <div class="hidden md:block flex justify-around">
            <a class="mr-4" href="#home">Home</a>
            <a class="mr-4" href="#about">About</a>
            <a class="mr-4 relative" href="#promotion">Promotion <span class="hot-css">HOT</span></a>
            <a class="mr-4" href="#blogs">Blogs</a>
            <a  class="mr-4" href="#contactus">Contact Us</a>
        </div>
    </nav>


    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
        <div class="md:pr-20 flex items-end">
            <p class="text-4xl mb-10 md:mb-0 md:text-6xl font-semibold txt--green">
                Good Food Us<br> Good Mood
            </p>
        </div>

        <div class="row-span-2 navbar__hero-img">
            <div class="flex justify-center items-center relative">
                <img class="navbar__hero-img-1" src="~/assets/img/content/shadow.png" alt="">
                <img class="absolute navbar__hero-img-2" src="~/assets/img/content/menu.png" alt="">
                <img class="hidden md:block absolute -bottom-7 -left-14" src="~/assets/img/content/rounded-image.png" alt="">
            </div>
        </div>

        <!-- description and CTA -->
        <div class="md:pr-20">
            <p class="mb-7">
                I would think that conserving our natural resources<br> should be a conservative position. Not to waste food, and<br> not to throw away a lot of the food that we buy.
            </p>

            <!-- CTA -->
            <div class="flex">   
                <button-base :buttonText="'Daftar Sekarang'" :type="'btn--green text-white mr-4'"></button-base>
                <button-base :buttonText="'About Us'" :type="'btn--abu'"></button-base>
            </div>
            
        </div>
    </div>



    <!-- navigasi mobile -->
    <div class="fixed md:hidden flex justify-around inset-x-0 bottom-0 py-3 bg-white">
        <div>
            <!-- logo -->
            <a href=""></a>

            <a href="">Home</a>
        </div>
        <div>
            <!-- logo -->
            <a href=""></a>

            <a href="">Promotions</a>
        </div>
        <div>
            <!-- logo -->
            <a href=""></a>

            <a href="">Others</a>
        </div>
    </div>
  </div>
</template>

<script>
import ButtonBase from './main-content/ButtonBase.vue'
export default {
  components: { ButtonBase },

}
</script>

<style>

</style>