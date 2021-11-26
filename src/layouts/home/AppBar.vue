<template>
  
    <v-app-bar
      id="home-app-bar"
      app
      height="150">
        <v-container>
          <v-row justify="center">
           <v-img
              :src="require('@/assets/sammy_logo.jpg')"
              class="mr-3"
              max-height="150"
             
            />
          </v-row>
          <v-row no-gutters>
            <v-col cols="12" class="text-center">
              
            </v-col>
          </v-row>
        </v-container>


    </v-app-bar>
 
</template>

<script>
  export default {
    name: 'HomeAppBar',

    data: () => ({
      drawer: null,
      items: [
        'Home',
        'Pro',
      ],
    }),
  }
</script>

<style lang="sass">
  #home-app-bar
    .v-tabs-slider
      max-width: 24px
      margin: 0 auto

    .v-tab
      &::before
        display: none
</style>
