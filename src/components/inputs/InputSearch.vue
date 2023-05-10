<template>
  <div class="relative text-white">
    <input type="text" class="w-full bg-gray-700 placeholder-white px-4 py-2 rounded-lg opacity-30 focus:opacity-60 outline-none focus:outline-none pr-10" placeholder="Search" />
    <SearchIcon class="w-4 h-4 absolute top-2 right-2.5" />
  </div>
</template>

<script>
import SearchIcon from "../icons/SearchIcon.vue";

export default {
  components: { SearchIcon },
};
</script>
