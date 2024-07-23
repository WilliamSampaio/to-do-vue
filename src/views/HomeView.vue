<template>
  <v-navigation-drawer v-model="drawer">
    <!--  -->
  </v-navigation-drawer>

  <v-app-bar>
    <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>

    <v-app-bar-title>Application</v-app-bar-title>
  </v-app-bar>

  <v-main>
    <h3>home</h3>
  </v-main>
  <FooterComponent />
</template>

<script setup>
import { ref } from 'vue'

const drawer = ref(null)
</script>

<script>
import FooterComponent from '../components/FooterComponent.vue'

export default {
  components: {
    FooterComponent
  },
  data: () => ({ drawer: null })
}
</script>
