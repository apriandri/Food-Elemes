<template>
  <div>
    <header>
      <v-header></v-header>
    </header>

    <main class="container mx-auto px-7">
      <v-section :mainTitle="'Browser Our Category'">
        <template v-slot:mainMenus>
          <div class="flex flex-row mb-5">
            <div v-for="(item, index) in itemCat" :key="index">
              <card-base :type="'cat-card-item'">
                <div class="flex flex-col justify-center items-center">
                  <div class="mb-10 mt-2">
                    <img
                      class="w-16"
                      :src="require(`../assets/img/category/kebab.svg`)"
                      alt=""
                    />
                  </div>
                  <p>
                    {{ item.name }}
                  </p>
                  <p>
                    {{ item.qty ? item.qty + "items" : "" }}
                  </p>
                </div>
              </card-base>
            </div>
          </div>

          <div class="flex justify-end">
            <button-base class="btn--green text-white rounded-full mr-3">
              <span class="bg-green-lighter txt--green rounded-full">
              </span>
              PREV</button-base
            >
            <button-base class="btn--green text-white rounded-full" >
              NEXT 
              <span class="bg-green-lighter txt--green rounded-full">
              </span>
            </button-base>
          </div>
        </template>
      </v-section>

      <v-section :mainTitle="'Browser Our Trending'" class="section__trending">
        <template v-slot:mainMenus>
          <div class="grid grid-cols-1 md:grid-cols-4 gap-4 mb-16">
            <card-base :type="'section__trending-card background-green-2-2'">
              <div>
                <img
                  class="section__trending-img"
                  src="~/assets/img/trending/pexels-alena-shekhovtcova-6940978 1.png"
                  alt=""
                />

                <div>
                  <p class="font-semibold text-lg">Pizza Paperoni</p>
                  <p class="txt--green text-sm">Pizza</p>
                  <img
                  class="stars"
                  src="~/assets/img/star.svg"
                  alt="" height="68.23px"
                />
                </div>
              </div>
            </card-base>

            <card-base :type="'section__trending-card bg-green-lighter'">
              <div>
                <img
                  class="section__trending-img"
                  src="~/assets/img/trending/pexels-daria-shevtsova-1260968 1.png"
                  alt=""
                />

                <div>
                  <p class="font-semibold text-lg">Pizza Meat</p>
                  <p class="txt--green text-sm">Pizza</p>
                   <img
                  class="stars"
                  src="~/assets/img/star-2.svg"
                  alt="" height="68.23px"
                />
                </div>
              </div>
            </card-base>

            <card-base :type="'section__trending-card background-red-1-2'">
              <div>
                <img
                  class="section__trending-img"
                  src="~/assets/img/trending/pexels-brett-jordan-842519 1.png"
                  alt=""
                />

                <div>
                  <p class="font-semibold text-lg">Pizza Paperoni</p>
                  <p class="txt--green text-sm">Pizza</p>
                   <img
                  class="stars"
                  src="~/assets/img/star-2.svg"
                  alt="" height="68.23px"
                />
                </div>
              </div>
            </card-base>

            <card-base :type="'section__trending-card background-blue-1-2'">
              <div>
                <img
                  class="section__trending-img"
                  src="~/assets/img/trending/pexels-olga-lioncat-7245464 1.png"
                  alt=""
                />

                <div>
                  <p class="font-semibold text-lg">Salmon Roll</p>
                  <p class="txt--green text-sm">Salmon</p>
                   <img
                  class="stars"
                  src="~/assets/img/star-2.svg"
                  alt="" height="68.23px"
                />
                </div>
              </div>
            </card-base>

            <card-base :type="'section__trending-card background-green-2-2'">
              <div>
                <img
                  class="section__trending-img"
                  src="~/assets/img/trending/pexels-nishant-aneja-2955819 1.png"
                  alt=""
                />

                <div>
                  <p class="font-semibold text-lg">Doner Kebab</p>
                  <p class="txt--green text-sm">Kebab</p>
                    <img
                  class="stars"
                  src="~/assets/img/star.svg"
                  alt="" height="68.23px"
                />
                </div>
              </div>
            </card-base>

            <card-base :type="'section__trending-card background-blue-1-2'">
              <div>
                <img
                  class="section__trending-img"
                  src="~/assets/img/trending/pexels-oleg-magni-1908674 1.png"
                  alt=""
                />

                <div>
                  <p class="font-semibold text-lg">Cupcake Choco</p>
                  <p class="txt--green text-sm">Cupcake</p>
                    <img
                  class="stars"
                  src="~/assets/img/star-2.svg"
                  alt="" height="68.23px"
                />
                </div>
              </div>
            </card-base>

            <card-base :type="'section__trending-card background-green-2-2'">
              <div>
                <img
                  class="section__trending-img"
                  src="~/assets/img/trending/pexels-karley-saagi-2064449 1.png"
                  alt=""
                />

                <div>
                  <p class="font-semibold text-lg">Doughnut Unicorn</p>
                  <p class="txt--green text-sm">Doughnut</p>
                   <img
                  class="stars"
                  src="~/assets/img/star-2.svg"
                  alt="" height="68.23px"
                />
                </div>
              </div>
            </card-base>

            <card-base :type="'section__trending-card background-blue-1-2'">
              <div>
                <img
                  class="section__trending-img"
                  src="~/assets/img/trending/pexels-polina-tankilevitch-6419736 1.png"
                  alt=""
                />

                <div>
                  <p class="font-semibold text-lg">Kathi Kebab</p>
                  <p class="txt--green text-sm">Kebab</p>
                    <img
                  class="stars"
                  src="~/assets/img/star.svg"
                  alt="" height="68.23px"
                />
                </div>
              </div>
            </card-base>
          </div>

          <div class="md:flex justify-center hidden">
            <button-base
              :buttonText="'ALL Receipt'"
              :type="'btn--green text-white'"
            ></button-base>
          </div>
        </template>
      </v-section>
    </main>

    <footer class="hidden md:block footer rounded-lg container mx-auto px-7" style="background-color: #F8FFF5">
      <v-footer></v-footer>
    </footer>
    <div class="mx-auto py-4">
      <center>
        <h1 class="text-sm">© 2021 Apri Andri. All rights reserved</h1>
      </center>
    </div>
  </div>
</template>

<script>
import CardBase from "~/components/main-content/CardBase.vue";
import ButtonBase from "~/components/main-content/ButtonBase.vue";
import VHeader from "~/components/VHeader.vue";
import VSection from "~/components/VSection.vue";
import VFooter from "~/components/VFooter.vue";
export default {
  components: { ButtonBase, CardBase, VHeader, VSection, VFooter },
  data() {
    return {
      currentIndex: 0,
      indexSlide: 0,
      itemCat: [
        {
          id: 1,
          name: "Cupcake",
          qty: 12,
          img: "pizza.svg",
        },
        {
          id: 2,
          name: "Pizza",
          qty: 15,
          img: "pizza.svg",
        },
        {
          id: 3,
          name: "Kebab",
          qty: 2,
          img: "kebab.svg",
        },
        {
          id: 4,
          name: "Salmon",
          qty: 42,
          img: "salmon.svg",
        },
         {
          id: 4,
          name: "Salmon",
          qty: 42,
          img: "salmon.svg",
        },
         {
          id: 4,
          name: "Salmon",
          qty: 42,
          img: "salmon.svg",
        },
      ],
    };
  },

  methods: {},
};
</script>
