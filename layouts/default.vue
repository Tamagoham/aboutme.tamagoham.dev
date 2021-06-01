<template>
  <v-app id="inspire">
    <!--  バーは必要ある？
    <v-app-bar
      app
      color="blue"
      flat
    >
      <v-container class="py-0 fill-height">
        <v-avatar
          class="mr-10"
          color="grey darken-1"
          size="32"
        ></v-avatar>

        <v-btn
          v-for="link in links"
          :key="link"
          text
        >
          {{ link }}
        </v-btn>

        <v-spacer></v-spacer>

        <v-responsive max-width="260">
          <v-text-field
            dense
            flat
            hide-details
            rounded
            solo-inverted
          ></v-text-field>
        </v-responsive>
      </v-container>
    </v-app-bar>
    -->

    <v-main class="grey lighten-3">
      <Particles
        id="tsparticles"
        :particles-init="particlesInit"
        :particles-loaded="particlesLoaded"
        url="./particlesjs-config.json"
      />
      <v-sheet
        min-height="100%"
      >
        <nuxt />
      </v-sheet>
    </v-main>
  </v-app>
</template>

<script>
import Vue from 'vue'
import Particles from 'particles.vue'
Vue.use(Particles)

export default {
  data: () => ({
    links: ['ホーム', 'ブログ', 'Twitter', 'GitHub']
  })
}
</script>

<style>
#tsparticles canvas {
  position: absolute;
  width: 100%;
  height: 100%;
  z-index: 0;
}
</style>
