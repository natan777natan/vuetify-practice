<template>
  <v-content>
    <v-container>
    <v-layout wrap>
      <v-flex xs12 sm6 md4 text-center my-5><v-btn>押して</v-btn></v-flex>
      <v-flex xs12 sm6 md4 text-center my-5><v-btn >押して</v-btn></v-flex>
      <v-flex xs12 sm6 md4 text-center my-5><v-btn>押して</v-btn></v-flex>
    </v-layout>
    </v-container>
  </v-content>
</template>



<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'


export default {
  components: {
    Logo,
    VuetifyLogo,
  }
}
</script>
