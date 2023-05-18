<template>
  <div class="bg-black bg-opacity-20 rounded-3xl overflow-hidden">
    <div class="header">
      <div class="h-32 w-full flex">
        <img src="/imagens/cake-morango.jpeg" class="w-full h-full object-cover"/>
      </div>
    </div>

    <div class="bg-purple-800 body relative p-5">
      <Avatar
        class="w-12 h-12 absolute right-2 -top-5 rounded-full overflow-hidden"
      />
      <h5 class="text-xs mb-2 opacity-50">
        Bela Doceria
        <div class="w-2 h-2 inline-block ml-2 rounded-full bg-green-400"></div>
      </h5>
      <p>Cake de morango</p>
      
      <div class="text-xs flex items-center space-x-3 opacity-50 mt-3">
        <span>50 visualizações</span>
        <span class="w-1 h-1 rounded-full bg-gray-300"></span>
        <span>2 semanas atrás</span>
      </div>
    </div>
  </div>
</template>

<script>
import Avatar from "./Avatar.vue";

export default {
  components: {
    Avatar,
  },
};
</script>
