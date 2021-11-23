<template>
 <v-row
    no-gutters
    class="authentication"
  >
   <v-col
     cols="12"
     sm="6"
    >
    <v-card
      elevation="13"
      class="authentication-card-form"
      >
      <v-card-title
        class="authentication-header"
      >
        <img
          src="@/assets/logoBrecho.png"
          alt="logo"
          class="authentication-logo"
        >
        <h1
          class="authentication-title"
        >
          Meu brechó.com
        </h1>
      </v-card-title>
      <v-card-text>
        <v-row
          class="authentication__form-container"
        >
          <v-col
            cols="12"
            md="9"
            lg="6"
          >
            <authentication-form :is-login="true"/>
          </v-col>
        </v-row>
      </v-card-text>
    </v-card>
   </v-col>
 </v-row>
</template>

<script>
import AuthenticationForm from '@/components/AuthenticationForm'

export default {
  components: {
    AuthenticationForm,
  },

}
</script>

<style lang="sass" scoped>
.authentication
  width: 100vw
  height: 100vh
  background: linear-gradient(90deg, #FFF 50%, rgba(255,255,255,0) 50%), var(--v-secondary-base)
  display: flex
  justify-content: center
  align-items: center

.authentication-card-form
  display: flex
  flex-direction: column

.authentication-header
  display: flex
  flex-direction: column
  place-items: center

.authentication-logo
  width: 100px

.authentication-title
  font-size: 2rem

.authentication__form-container
  display: flex
  justify-content: center

</style>
