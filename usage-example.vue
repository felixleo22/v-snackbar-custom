<template>
  <div class="text-center">
    <v-btn dark color="orange darken-2" @click="exampleSnack">
      button
    </v-btn>
     <v-btn dark color="orange darken-2" @click="errorSnack">
      open Snackbar
    </v-btn>
    <v-btn dark color="orange darken-2" @click="customSnack">
      custom button
    </v-btn>
  </div>
</template>

<script>
export default {
  name: "example",
  data: () => {
    return {
    };
  },
  methods: {
    exampleSnack () {
      this.$store.dispatch('snacks/info', 'put your text here')
    },
    errorSnack () {
      this.$store.dispatch('snacks/error', 'error button')
    },
    customSnack () {
      this.$store.dispatch('snacks/info', { text: 'firt button', color: yellow })
    }
  }
};
</script>
