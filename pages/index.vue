<template>
  <v-app>
    <div id="app">
      <v-container id="container">
        <v-col>
          <v-card
            :loading="loading"
            class="mx-auto my-12 rounded-xl"
            max-width="890px"
          >
            <v-row justify="space-around" class="pt-md-5">
              <v-avatar size="250" class="text-center">
                <img
                  src="https://avatars.githubusercontent.com/u/19357599?v=4"
                  alt="Tamagoham"
                />
              </v-avatar>
            </v-row>
            <v-card-title class="justify-center text-h4">
              Tamagoham
            </v-card-title>

            <v-card-subtitle class="text-center text-h6">
              (Yuzuru Naito)
            </v-card-subtitle>

            <v-card-text class="text-center text-h6">
              Ritsumeikan University - Information Science and Engineering<br>
              立命館大学 情報理工学部
            </v-card-text>
            <v-divider class="mx-4 mt-md-5 mb-md-5"></v-divider>

            <v-card-title class="justify-center">Follow Me!!</v-card-title>

            <v-card-text class="text-center text-h6">
              <v-row>
                <v-col>
                  <v-btn
                    x-large
                    color="success"
                    dark
                    min-height="80px"
                    outlined
                    href="https://github.com/Tamagoham"
                    target="_blank"
                  >
                    <v-icon size="70px">mdi-github</v-icon>
                    <div class="text-h6 pl-md-2">GitHub</div>
                  </v-btn>
                </v-col>
                <v-col>
                  <v-btn
                    x-large
                    color="success"
                    dark
                    min-height="80px"
                    outlined
                    href="https://twitter.com/yzr_7110"
                    target="_blank"
                  >
                    <v-icon size="70px">mdi-twitter</v-icon>
                    <div class="text-h6 pl-md-2">Twitter</div>
                  </v-btn>
                </v-col>
                <v-col>
                  <v-btn
                    x-large
                    color="success"
                    dark
                    min-height="80px"
                    outlined
                    href="https://instagram.com/yzr_7110"
                    target="_blank"
                  >
                    <v-icon size="70px">mdi-instagram</v-icon>
                    <div class="text-h6 pl-md-2">Instagram</div>
                  </v-btn>
                </v-col>
              </v-row>
            </v-card-text>
            <v-divider class="mx-4 mt-md-7 mb-md-7"></v-divider>
            <v-card-title class="justify-center">Skills</v-card-title>

            <v-card-text class="text-center text-h6">
              <v-row
                class="pt-md-5 pl-md-5 pr-md-5"
                justify="center"
                align-content="center"
              >
                <v-col>
                  <v-card class="mx-auto" max-width="170" outlined>
                    <v-list-item three-line>
                      <v-list-item-content>
                        <v-row justify="space-around" class="pt-md-3 pb-md-3">
                          <v-img
                            contain
                            max-width="130"
                            max-height="50"
                            src="logo/php.svg"
                          ></v-img>
                        </v-row>
                        <v-list-item-title class="text-h5 mb-1">
                          PHP
                        </v-list-item-title>
                        <v-list-item-subtitle>
                          Laravel, Composer
                        </v-list-item-subtitle>
                      </v-list-item-content>
                    </v-list-item>
                  </v-card>
                </v-col>
                <v-col>
                  <v-card class="mx-auto" max-width="170" outlined>
                    <v-list-item three-line>
                      <v-list-item-content>
                        <v-row justify="space-around" class="pt-md-3 pb-md-3">
                          <v-img
                            contain
                            max-width="130"
                            max-height="50"
                            src="logo/c.svg"
                          ></v-img>
                        </v-row>
                        <v-list-item-title class="text-h5 mb-1">
                          C
                        </v-list-item-title>
                        <v-list-item-subtitle>
                          基本的なところ。
                        </v-list-item-subtitle>
                      </v-list-item-content>
                    </v-list-item>
                  </v-card>
                </v-col>
                <v-col>
                  <v-card class="mx-auto" max-width="170" outlined>
                    <v-list-item three-line>
                      <v-list-item-content>
                        <v-row justify="space-around" class="pt-md-3 pb-md-3">
                          <v-img
                            contain
                            max-width="130"
                            min-height="50"
                            max-height="50"
                            src="logo/python.png"
                          ></v-img>
                        </v-row>
                        <v-list-item-title class="text-h5 mb-1">
                          Python
                        </v-list-item-title>
                        <v-list-item-subtitle>
                          OpenCV, numpy
                        </v-list-item-subtitle>
                      </v-list-item-content>
                    </v-list-item>
                  </v-card>
                </v-col>
                <v-col>
                  <v-card class="mx-auto" max-width="170" outlined>
                    <v-list-item three-line>
                      <v-list-item-content>
                        <v-row justify="space-around" class="pt-md-3 pb-md-3">
                          <v-img
                            contain
                            max-width="150"
                            min-height="50"
                            max-height="50"
                            src="logo/tensorflow.svg"
                          ></v-img>
                        </v-row>
                        <v-list-item-title class="text-h5 mb-1">
                          Tensorflow
                        </v-list-item-title>
                        <v-list-item-subtitle> CNN, RNN </v-list-item-subtitle>
                      </v-list-item-content>
                    </v-list-item>
                  </v-card>
                </v-col>
              </v-row>
              <v-row
                class="pb-md-5 pl-md-5 pr-md-5"
                justify="center"
                align-content="center"
              >
                <v-col>
                  <v-card class="mx-auto" max-width="170" outlined>
                    <v-list-item three-line>
                      <v-list-item-content>
                        <v-row justify="space-around" class="pt-md-3 pb-md-3">
                          <v-img
                            contain
                            max-width="130"
                            max-height="50"
                            min-height="50"
                            src="logo/nuxtjs.svg"
                          ></v-img>
                        </v-row>
                        <v-list-item-title class="text-h5 mb-1">
                          Nuxt.js
                        </v-list-item-title>
                        <v-list-item-subtitle>
                          このサイトもこれで
                        </v-list-item-subtitle>
                      </v-list-item-content>
                    </v-list-item>
                  </v-card>
                </v-col>
                <v-col>
                  <v-card class="mx-auto" max-width="170" outlined>
                    <v-list-item three-line>
                      <v-list-item-content>
                        <v-row justify="space-around" class="pt-md-3 pb-md-3">
                          <v-img
                            contain
                            max-width="130"
                            max-height="50"
                            min-height="50"
                            src="logo/html5.svg"
                          ></v-img>
                        </v-row>
                        <v-list-item-title class="text-h5 mb-1">
                          HTML
                        </v-list-item-title>
                        <v-list-item-subtitle>
                          ※センスなし
                        </v-list-item-subtitle>
                      </v-list-item-content>
                    </v-list-item>
                  </v-card>
                </v-col>
              </v-row>
            </v-card-text>
            <v-divider class="mx-4 mt-md-5 mb-md-5"></v-divider>

            <v-card-title class="justify-center">Thank you!</v-card-title>
            <v-divider class="mx-4 mt-md-5 mb-md-5"></v-divider>
          </v-card>
        </v-col>
      </v-container>
    </div>
  </v-app>
</template>



<script>
import Vue from "vue";
import Logo from "~/components/Logo.vue";
import VuetifyLogo from "~/components/VuetifyLogo.vue";

export default {
  components: {
    Logo,
    VuetifyLogo,
  },
};
</script>
