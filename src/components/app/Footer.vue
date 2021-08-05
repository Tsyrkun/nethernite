<template>
  <v-card
    class="flex"
    flat
    tile
  >
    <v-card-title class="teal">
      <strong class="subheading">Get connected with me on social networks!</strong>

      <v-spacer></v-spacer>

      <v-btn
        v-for="social in socials"
        :key="social.icon"
        class="mx-4"
        dark
        icon
        target="_blank"
        :href="social.url"
      >
        <v-icon size="24px">
          {{ social.icon }}
        </v-icon>
      </v-btn>
    </v-card-title>

    <v-card-text class="py-2 white--text text-center">
      {{ new Date().getFullYear() }} — <strong>Vlad Tsyrkun</strong>
    </v-card-text>
  </v-card>
</template>

<script>
export default {
  name: 'Footer',
  data: () => ({
    socials: [
      {
        icon: 'mdi-github-circle',
        url: 'https://github.com/tsyrkun',
      },
      {
        icon: 'mdi-linkedin',
        url: 'https://www.linkedin.com/in/vlad-tsyrkun',
      },
    ],
  }),
};
</script>

<style scoped>

</style>
