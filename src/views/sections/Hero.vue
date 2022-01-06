<template>
  <section id="hero">
    <v-img
      :min-height="minHeight"
      :src="require('@/assets/vegan-food.jpg')"
      class="white--text"
      gradient="to bottom, rgba(20, 20, 20, .4), rgba(0,0,0,.3)"
    >
      <v-container class="px-2 py-0">
        <v-responsive
          class="d-flex align-center mx-auto"
          height="50%"
          max-width="800"
          width="90%"
        >
        <br/><br/><br/>
        <v-card class="rounded-xl" color="#0000004D">
          <br/><br/>
          <v-row class="mx-6" align="center">
            <base-subheading
            size="text-h5"
            weight="regular"
            title="Veganismo é a grande ferramenta para transformar o mundo!"  
            />
            <base-body >
              <p class="text-white">O ser humano por séculos tem se desconectado da natureza e por consequência lógica também se afastou das relações de compaixão pela terra e seus seres.</p>
              <p class="text-white">O termo vegano já existe desde 1944 e foi criado pelo britânico Donald Watson e, desde então, transformou-se em um movimento político, ético e de estilo de vida, e vem ganhando muitos adeptos, mas hoje não é apenas isso, o veganismo é o futuro que construímos agora.</p> 
              <p class="text-white">Meu compromisso como especialista em gastronomia exclusivamente plant based é pensar, expressar e praticar o veganismo como forma de ampliar a consciência de forma leve, divertida e saborosa.</p>
              <p class="text-white">Ainda há muito a percorrer para um mundo mais equilibrado e sustentável, mas tenho certeza que de mãos dadas podemos encurtar esse caminho.</p>
              <p class="text-white">Vamos viver essa experiência juntos?</p>
            </base-body>
          </v-row>
        </v-card>
        <br/><br/><br/><br/>
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
        const height = this.$vuetify.breakpoint.mdAndUp ? '50vh' : '25vh'

        return `calc(${height} - ${this.$vuetify.application.top}px)`
      },
    },
  }
</script>
<style type="text/css">
  rounded-card{
      border-radius:60;
  }
  p{
      color:white;
  }

</style>
