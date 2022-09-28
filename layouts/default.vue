<template>
  <!-- App.vue -->

  <v-app>

    <v-app-bar app clipped-left>
      <v-btn @click="toggleTheme">toggle theme</v-btn>
    </v-app-bar>

    <!-- Sizes your content based upon application components -->
    <v-main>

      <!-- Provides the application the proper gutter -->
      <v-container>

        <!-- If using vue-router -->
        <!-- <router-view></router-view> -->
        A *default* layout
        <slot />

      </v-container>
    </v-main>


    <v-footer app>
      <!-- -->
    </v-footer>

  </v-app>

</template>

<script>
import { useTheme } from 'vuetify'

export default {
  name: "default.vue",

  data() {
    return {
      mini: false,
      navbar: true
    }
  },
  setup() {
    const theme = useTheme()

    return {
      theme,
      toggleTheme: () => theme.global.name.value = theme.global.current.value.dark ? 'light' : 'dark'
    }
  }
}
</script>
