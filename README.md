# v-snackbar-component-custom

```js
<template>
  <div class="text-center">
    <v-btn dark color="orange darken-2" @click="action">
      button
    </v-btn>
  </div>
</template>

<script>
export default {
  name: "example",
  data: () => {
    return {};
  },
  methods: {
    action () {
      // use like this
      this.$store.dispatch('snacks/info', 'put your test here')
    },
  }
};
</script>
```
## Prerequisites
* vue / nuxt
* vuetify
* mdi-icon
* vuex



To use the snackbars in this way:

- Place the `Snackbar.vue` file in your `components` folder
- Place the `snacks.vue` file in your `store` folder
- Add in your `layouts` file the custom component
- Let's use it everywhere :)

