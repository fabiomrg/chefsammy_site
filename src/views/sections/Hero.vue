<template>
  <section id="hero">
    <v-img
      :min-height="minHeight"
      :src="require('@/assets/light.jpg')"
      class="white--text"
      gradient="to bottom, rgba(20, 20, 20, .9), rgba(0,0,0,.6)"
    >
      <v-container class="px-4 py-12">
        <v-responsive
          class="d-flex align-center mx-auto"
          height="100%"
          max-width="600"
          width="90%"
        >
        <br/>
          <base-subheading
          size="text-h5"
          weight="regular"
          title="CELEBRE A UNIÃO, A VITÓRIA, OS ENCONTROS, OS REENCONTROS E A VIDA..."  
         />

          <base-heading
             size="text-h2"
            title="...COM MUITO AMOR!"
            weight="medium"
          />

          <base-body>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Repudiandae nobis neque aspernatur in quas iure id aliquid, esse debitis, quibusdam mollitia! Quia ea expedita magnam totam, earum omnis et perspiciatis?
          </base-body>

        </v-responsive>
      </v-container>
    </v-img>
  </section>
</template>

<script>
  export default {
    name: 'SectionHero',

    provide: {
      theme: { isDark: true },
    },

    computed: {
      minHeight () {
        const height = this.$vuetify.breakpoint.mdAndUp ? '100vh' : '50vh'

        return `calc(${height} - ${this.$vuetify.application.top}px)`
      },
    },
  }
</script>
