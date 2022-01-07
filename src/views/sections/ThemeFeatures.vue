<template>
  <base-section id="servicos">
  
    <base-section-heading title="Serviços">
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
            {{text}}
          </base-avatar-card>
        </v-col>
      </v-row>
    </v-container><br/>
    <div id="cursos" style="background-color: #e4e4e4">
      <br/><br/><br/>
      <base-section-heading title="Cursos e Treinamentos">
        <v-row class="mx-6" align="center">
        <b>Aprenda a criar e preparar pratos nutritivos, deliciosos e 100% veganos.
          Cursos presenciais: </b>
        </v-row>
      </base-section-heading>
      <v-container>
          <v-row>
            <v-col
              v-for="(master, i) in masterclass"
              :key="i"
              cols="12"
              md="6"
            >
              <base-avatar-card
                v-bind="master"
                align="left"
                horizontal
              >
                {{text}}
              </base-avatar-card>
            </v-col>
          </v-row>
      </v-container><br/>
      <br/><br/>
    </div>
    
    <div id="consultoria" >
      <br/><br/><br/>
     <base-section-heading title="Consultoria para Restaurantes">
      <v-row class="mx-6" align="center">
          <b>O veganismo veio para ficar e seu restaurante não pode ficar fora!</b>
      </v-row>
     </base-section-heading>
    <v-container>
      <v-row>
        <v-col
          v-for="(consult, i) in consulting"
          :key="i"
          cols="12"
          md="6"
        >
          <base-avatar-card
            v-bind="consult"
            align="left"
            horizontal
          >
            {{text}}
          </base-avatar-card>
        </v-col>
      </v-row>
    </v-container><br/><br/><br/>
    </div>
  
   <div id="about" style="background-color: #e4e4e4">
     <br/><br/>
    <base-section-heading title="Sammy Gonzalez">
        <div class="d-flex flex-column justify-space-between align-center">
        <v-img 
          max-width="350"
          :src="require('@/assets/sammy.jpg')"
          
          ></v-img>
        </div>
        <br/><br/>
        <v-row class="mx-6" align="center">
        Sou Sammy Gonzalez, crio e preparo pratos veganos, busco sempre surpreender com experiências sensoriais que marquem, valorizem e estimulem a apreciação da alimentação a base de plantas. Predominantemente utilizo produtos orgânicos vindos de pequenos produtores e da agricultura familiar.
        </v-row>
      </base-section-heading>
      <br/>
   </div>
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
          text:'Seja uma produção de um filme, um curso, uma roda de conversas, uma palestra, tenho o serviço certo para seus eventos! Consulte os formatos de atendimento!'
        },
    
        {
          title: 'Jantares ou almoços',
          icon: 'mdi-pasta',
          text:'Posso preparar tudo no local com garçom e tudo ou também levo  pronto para algo mais intimista e ter uma experiência inesquecível.'
        },
          {
          title: 'Buffet de Casamento',
          icon: 'mdi-ring',
          text: 'A celebração da sagrada união de duas almas para trilhar uma jornada tão importante merece uma alimentação alinhada com os novos tempos. Cardápio sensível e personalizado como a ocasião merece e surpreender seus convidados! Atendo São Paulo e interior! Levamos tudo o que é necessário para um cuidado preciso: Material, serviço, respeito e amor que ocasião merece!'

        },
        {
          title: 'Aniversários',
          icon: 'mdi-account-star',
          text: 'Nada como festejar o início de uma nova jornada conectados à natureza e sua constante manifestação da vida! Celebre com um cardápio 100% vegano (plant based) preparado com ingredientes maravilhosos que a sagrada terra nos presenteia em sua perfeição!'

        },
        
        {
          title: 'Kit picnic',
          icon: 'mdi-food-apple',
          text: 'Uma experiência especial ao ar livre em conexão com a natureza e liberdade que o momento nos proporciona! O cardápio kit picnic é levado em embalagens individuais e descartáveis para facilitar o manuseio! Consulte cardápio que pode ser quente ou frio!'

        },
        
        {
          title: 'Kit Escola',
          icon: 'mdi-town-hall',
          text: 'A escola é um dos momentos mais importantes da vida pois estamos iniciando nossa jornada de socialização e que sem dúvidas levamos para sempre em nossas memórias! Preparo kit individuais e descartáveis para facilitar a manipulação dos presentes com cardápio especial para o paladar infanto juvenil!Consulte opções de cardápio!'

        },

        {
          title: 'Corporativos',
          icon: 'mdi-account-tie',
          text: 'Reunião de negócios, apresentação de produtos, roda de conversas, treinamentos e celebrações! Consulte os formatos de atendimento!'

        },
        
        {
          title: 'Cestas especiais',
          icon: 'mdi-star',
          text: 'Surpreender e ser surpreendido com uma cesta incrível, com ingredientes saborosos e selecionados com delicadeza para elevar a experiência ao máximo! Consulte!'

        },
      ],

      masterclass: [
  
        {      
          title: '- Treinamento Personalizados',
          
          text:'Um treinamento específico para as necessidades do aprendiz é realizado em sua própria cozinha ou local de trabalho!  - Consulte. '
        },
    
        {
          title: '- Em grupos',
          
          text:'Curso de agenda mensal que pode ser 1, 2 ou 3 módulos! Acompanhe no instagram.'
        },
          {
          title: '- Online',
          
          text: 'Estou preparando uma deliciosa Masterclass de Bases da Gastronomia vegana! Em breve terei notícias do lançamento, acompanhe nas redes sociais!'

        },
        
      ],

      consulting: [
  
        {  
          title: '- Opções Veganas',    
          text: 'Introduza pratos deliciosamente veganos em seu cardápio!',
          
        },
    
        {
          title: '- Aprimoramento de receitas',
          text: 'Melhore suas receitas veganas e surpreenda seus clientes?',
          
        },
          {
          title: '- Entendendo o veganismo',
          text: 'Quer aprender sobre o mundo vegano, sustentabilidade e como atender este grupo que cresce exponencialmente a cada ano?',
          
          

        },
        
      ],

    }),
  }
</script>
