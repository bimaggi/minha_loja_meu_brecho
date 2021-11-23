<template>
  <v-app id="app">
      <v-main>
        <v-row no-gutters>
          <authentication />
        </v-row>
    </v-main>
  </v-app>
</template>

<script>
import Authentication from '@/views/Authentication'

export default {
  name: 'App',
  components: {
    Authentication,
  },

  data: () => ({
    //
  }),
}
</script>
