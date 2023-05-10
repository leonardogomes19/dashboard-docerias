
<template>
  <Dashboard/>
</template>

<script lang="js">
import { defineComponent } from 'vue';
import Dashboard from './layouts/Dashboard.vue';

export default defineComponent({
  name: 'App',
  components: {
    Dashboard
  },
  setup(){
    const name = 'Marco';
    return { name }
  }
})
</script>