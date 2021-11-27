<template>
  <base-section id="theme-features">
 
    <base-section-heading id="about" title="Sammy Gonzalez">
      <v-row justify="center">
        <v-img :src="require('@/assets/sammy.jpg')"
        
      ></v-img>
      </v-row>
      <br/>
      Sou Sammy Gonzalez, crio e preparo pratos veganos, busco sempre surpreender com experiências sensoriais que marquem, valorizem e estimulem a apreciação da alimentação a base de plantas. Predominantemente utilizo produtos orgânicos vindos de pequenos produtores e da agricultura familiar.
    </base-section-heading>
   
    <base-section-heading id="eventos" title="Eventos">
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
    <base-section-heading id="cursos" title="Cursos">
     Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis illum veniam cum dolores ratione commodi beatae quas maxime, laboriosam excepturi solut! Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis illum veniam cum dolores ratione commodi beatae quas maxime, laboriosam excepturi solut! Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis illum veniam cum dolores ratione commodi beatae quas maxime, laboriosam excepturi solut!
    </base-section-heading>
     <base-section-heading id="consultoria" title="Consultoria">
     Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis illum veniam cum dolores ratione commodi beatae quas maxime, laboriosam excepturi solut! Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis illum veniam cum dolores ratione commodi beatae quas maxime, laboriosam excepturi solut! Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis illum veniam cum dolores ratione commodi beatae quas maxime, laboriosam excepturi solut!
    </base-section-heading>
     <base-section-heading id="contatos" title="Contatos">
     Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis illum veniam cum dolores ratione commodi beatae quas maxime, laboriosam excepturi solut! Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis illum veniam cum dolores ratione commodi beatae quas maxime, laboriosam excepturi solut! Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis illum veniam cum dolores ratione commodi beatae quas maxime, laboriosam excepturi solut!
    </base-section-heading>
  </base-section>
  

</template>

<script>
  export default {
    name: 'SectionThemeFeatures',

    data: () => ({
      features: [
  
        {      
          title: 'Catering',
          
          icon: 'mdi-book-open-page-variant',
        },
        {
          title: 'Jantares',
          icon: 'mdi-pasta',
        },
          {
          title: 'Aniversários',
          icon: 'mdi-account-star',
        },
      ],
    }),
  }
</script>
