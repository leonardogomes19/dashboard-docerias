<template>
  <div class="bg-white flex text-white max-h-screen h-screen">
    <div class="bg-purple-900 w-64">
      <span class="font-semibold p-6 block opacity-90">Dashboard Docerias</span>

      <nav class="p-6">
        <h3
          class="opacity-50 uppercase font-semibold tracking-wider mb-3 text-xs"
        >
          Menu
        </h3>

        <div class="space-y-6">
          <MenuItems :icon="HomeIcon">Descubra</MenuItems>
          <MenuItems :icon="TrendingUpIcon">Em alta</MenuItems>
          <MenuItems :icon="TrendingUpIcon">Mais vendidos</MenuItems>
        </div>
      </nav>
    </div>

    <div class="flex-1 h-screen relative overflow-y-auto">
      <header
        class="flex p-5 bg-gray-800 z-20 sticky top-0 items-center justify-between"
      >
        <InputSearch class="w-96" />

        <div class="flex items-center">
          <div class="flex items-center space-x-3">
            <Avatar class="rounded-full overflow-hidden w-10 h-10" />

            <span>Thomas</span>
            <ChevronDownIcon class="w-4 h-4" />
          </div>

          <BellIcon
            class="w-5 h-5 ml-8 opacity-50 hover:opacity-100 cursor-pointer transition duration-100"
          />
        </div>
      </header>

      <h1 class="font-bold text-4xl ml-5 mt-6 mb-4 text-black">Destaques</h1>

      <div class="px-5 pb-5 content">
        <div class="grid gap-4 grid-cols-12">
          <div class="col-span-8 h-96 rounded-3xl overflow-hidden relative">
            <div class="flex w-full h-full">
              <img
                src="/imagens/cake.jpg"
                class="w-full object-cover"
              />
            </div>
            <div class="z-10 absolute top-0 p-6 w-full bottom-0">
              <h3 class="text-2xl max-w-xs">
                Cake
              </h3>

              <div
                class="absolute right-6 bottom-6 px-2 py-1 rounded-lg bg-gray-800 bg-opacity-50 text-white"
              >
                R$50.00
              </div>
            </div>
          </div>
          <div class="col-span-4 h-96 rounded-3xl overflow-hidden relative">
            <div class="flex w-full h-full">
              <img
                src="/imagens/pao-de-mel.jpg"
                class="w-full object-cover"
              />
            </div>
            <div class="z-10 absolute top-0 p-6 w-full bottom-0">
              <h3 class="text-2xl max-w-xs">
                Pão de Mel
              </h3>

              <div
                class="absolute right-6 bottom-6 px-2 py-1 rounded-lg bg-gray-800 bg-opacity-50 text-white"
              >
                R$10.00
              </div>
            </div>
          </div>
        </div>

        <h1 class="text-2xl mt-6 mb-4 text-black">Mais vistos</h1>
        <div class="grid grid-cols-4 gap-4">
          <CardItem v-for="(n, index) of 10" :key="index" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import HomeIcon from "../components/icons/HomeIcon.vue";
import TrendingUpIcon from "../components/icons/TrendingUpIcon.vue";
import ChevronDownIcon from "../components/icons/ChevronDownIcon.vue";
import BellIcon from "../components/icons/BellIcon.vue";
import MenuItems from "./navs/MenuItem.vue";
import InputSearch from "../components/inputs/InputSearch.vue";
import Avatar from "../components/Avatar.vue";
import CardItem from "../components/CardItem.vue";

export default {
  components: {
    HomeIcon,
    TrendingUpIcon,
    ChevronDownIcon,
    BellIcon,
    MenuItems,
    InputSearch,
    Avatar,
    CardItem,
  },
  data() {
    return {

    };
  },
};
</script>
