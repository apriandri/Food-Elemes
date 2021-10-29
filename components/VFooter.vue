<template>
  <div class="flex justify-around" style="padding: 1rem">
    <div class="m-3 footer__sec-1">
      <img src="~/assets/img/logo.png" alt="" class="mb-3" />

      <p class="mb-3 text-sm text-gray-500">
        Jl. Prof. DR. Satrio No.7, RT.3/RW.3, Karet Kuningan,<br> Kecamatan
        Setiabudi, Kota Jakarta Selatan, <br>Daerah Khusus Ibukota Jakarta 12950
      </p>

      <!-- icon -->
    </div>

    <div class="m-3 footer__sec-2">
      <h3 class="mb-3 font-semibold">Categories</h3>
      <ul class="text-sm text-gray-500">
        <li>
          <a href="">Cupcake</a>
        </li>
        <li>
          <a href="">Pizza</a>
        </li>
        <li>
          <a href="">Kebab</a>
        </li>
        <li>
          <a href="">Salmon</a>
        </li>
        <li>
          <a href="">Dognut</a>
        </li>
      </ul>
    </div>

    <!-- about us -->
    <div class="m-3 footer__sec-3">
      <h3 class="mb-3 font-semibold">About Us</h3>

      <ul class="text-sm text-gray-500">
        <li>
          <a href="">About Us</a>
        </li>
        <li>
          <a href="">FAQ</a>
        </li>
        <li>
          <a href="">Report Problem</a>
        </li>
      </ul>
    </div>

    <div class="m-3 footer__sec-4">
      <h3 class="mb-3 font-semibold">Newsletter</h3>
      <p class="text-sm text-gray-500 mb-3">
        Get now free 50% discount for alll products on your first order
      </p>
      <div class="flex mb-3">
        <input class="rounded-l-lg border" type="email" placeholder="Your email address"/>
        <button class="p-2 btn--green text-white text-xs rounded-r-lg">
          SEND
        </button>
      </div>
      <div>
        <ul>
          <li class="text-xs">
           <b> elemesid@gmail.com</b>
          </li>
          <li>
            0888 1111 2222
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
import ButtonBase from "./main-content/ButtonBase.vue";
export default {
  components: { ButtonBase },
};
</script>

<style>
</style>