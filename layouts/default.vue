<template>
  <v-app id="v-snackbar-component-custom">
  <Snackbar />
    <v-main>
      <v-container fluid>
        <nuxt />
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import Snackbar from '~/components/Snackbar.vue'

export default {
  components: {
    Snackbar
  }
}
</script>
