<template>
  <div class="flex items-center space-x-4">
    <div class="bg-orange-500 p-2 rounded-lg">
      <component :is="icon" class="w-4 h-4" />
    </div>

    <span>
      <slot></slot>
    </span>
  </div>
</template>

<script>
import HomeIcon from "../../components/icons/HomeIcon.vue";
import { defineProps } from "vue";
export default {
  components() {
    HomeIcon,
      defineProps({
        icon: { default: null },
      });
  },
};
</script>
