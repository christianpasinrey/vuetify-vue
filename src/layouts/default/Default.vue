<template>
  <v-app
    id="app"
    :dark="dark"
    :full-height="true"
    :full-width="true"
  >
    <default-bar>
      <template v-slot:content>
        <default-view />
      </template>
    </default-bar>
  </v-app>
</template>
<script setup>
  import DefaultBar from './AppBar.vue'
  import DefaultView from './View.vue'
  import { ref } from 'vue'
  const dark = ref(false)
</script>
