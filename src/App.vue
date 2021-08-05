<template>
  <v-app>
    <v-main>
      <router-view/>
    </v-main>
    <v-footer
      dark
      padless
      app
    >
      <Footer />
    </v-footer>
  </v-app>
</template>

<script>
import Footer from '@/components/app/Footer.vue';

export default {
  name: 'App',

  data: () => ({
    //
  }),
  components: {
    Footer,
  },
};
</script>
