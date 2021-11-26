<template>
  <base-section id="theme-features">
 
    <base-section-heading title="Sammy Gonzalez">
      <v-row justify="center">
        <v-img :src="require('@/assets/sammy.jpg')"
        
      ></v-img>
      </v-row>
      <br/>
      Sou Sammy Gonzalez, crio e preparo pratos veganos, busco sempre surpreender ... Libero, in! Asperiores, impedit libero. Veniam rerum saepe unde nihil possimus quibusdam esse accusamus mollitia magni fuga impedit libero. Veniam rerum saepe unde nihil possimus quibusdam esse accusamus mollitia magni fuga.
    </base-section-heading>
   
    
    <v-container>
      <v-row>
        <v-col
          v-for="(feature, i) in features"
          :key="i"
          cols="12"
          md="6"
        >
          <base-avatar-card
            v-bind="feature"
            align="left"
            horizontal
          >
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis illum veniam cum dolores ratione commodi beatae quas maxime, laboriosam excepturi solut!
          </base-avatar-card>
        </v-col>
      </v-row>
    </v-container>
  </base-section>
</template>

<script>
  export default {
    name: 'SectionThemeFeatures',

    data: () => ({
      features: [
  
        {      
          title: 'Realização de eventos',
          icon: 'mdi-pasta',
        },
        {
          title: 'Cursos de culinária',
          icon: 'mdi-book-open-page-variant',
        },
          {
          title: 'Consultoria',
          icon: 'mdi-account-star',
        },
      ],
    }),
  }
</script>
