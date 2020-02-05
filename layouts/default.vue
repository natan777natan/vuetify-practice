<template>
  <v-app>
    <!-- headerはじめ -->
    <Header />
    <!-- header終わり -->

    <!-- 本文内容 -->
    <nuxt />
    <!-- 本文内容終わり -->



    <!-- footerはじめ -->
    <Footer />
    <!-- footer終わり -->

  </v-app>
</template>

<script>
import Header from "@/components/Header";
import Footer from "@/components/Footer";
export default {
  components: {
    Header,
    Footer
  },
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  }
}
</script>
