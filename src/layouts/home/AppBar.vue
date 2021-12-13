<template>
  
    <v-app-bar
      id="home-app-bar"
      app
      elevation="1"
      height="130"
      >
        <home-menu/>

         <v-container>
        
          <v-row justify="center">
            <v-img 
              max-width="500"
              :src="require('@/assets/sammy_logo.jpg')"
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

    components: {
      
      HomeMenu: () => import('@/layouts/home/menu'),
    },
  }
</script>

<style lang="sass">
  #home-app-bar
    .v-tabs-slider
      max-width: 24px
      margin: 2 auto

    .v-tab
      &::before
        display: none
  #padding-zero
    .padding-zero

</style>
