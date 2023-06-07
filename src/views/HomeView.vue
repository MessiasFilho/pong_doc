<template>
    <div>
        <v-col cols="12" >
        <v-card  elevation="5" class="d-flex justify-center" >
           <v-img   src="../assets/tamb_3.png"></v-img> 
        </v-card>
    <v-card>
      <v-card class="mt-5 ml-3 mr-3" >
        <v-row justify="center">
          <v-expansion-panels accordion>
            <v-expansion-panel>
              <v-expansion-panel-header><v-toolbar-title>Introdução</v-toolbar-title> </v-expansion-panel-header>
              <v-expansion-panel-content>
          
                <v-card-text>
                  Este é um projeto de faculdade, desenvolvido para apresentarmos a uma empresa de games.
                  O jogo pong é um dos pioneiros quando falamos de jogos digitais, aproveitando a ideia de reproduzir um dos primeiros jogos criado resolvemos usar um ambiente mais retrô para o nosso projeto, usando como base também gráficos, designs e até personagens de um outro jogo bem clássico. 
                </v-card-text>
               
              </v-expansion-panel-content>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-row>
        </v-card>
      <v-card class="mt-5 ml-3 mr-3" >
        <v-row justify="center">
          <v-expansion-panels accordion>
            <v-expansion-panel>
              <v-expansion-panel-header><v-toolbar-title>Em que foi inspirado</v-toolbar-title> </v-expansion-panel-header>
              <v-expansion-panel-content>
          
                <v-card-text>
                  O jogo é inspirado no pingue pongue, implementamos figuras do jogo mortal kombat e tivemos a ideia de usar o nome mortal pong usando assim no lugar de pontos, life assim cada ponto indo a diminuir o life de vida do rival, ganhando quem finalizar a vida do outro primeiro.
                </v-card-text>
               
              </v-expansion-panel-content>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-row>
        </v-card>
      <v-card class="mt-5 ml-3 mr-3" >
        <v-row justify="center">
          <v-expansion-panels accordion>
            <v-expansion-panel>
              <v-expansion-panel-header><v-toolbar-title>Nosso Projeto</v-toolbar-title> </v-expansion-panel-header>
              <v-expansion-panel-content>
          
                <v-card-text>
                  A equipe é composta por 10 pessoas, onde foi dividida em 7 funções. Após debates para definir o que iriamos fazer, ficou decidido refazer o jogo Pong com melhorias.
                </v-card-text>
                <v-card-text>
                  Com o nosso projeto pretendemos impactá-los com algumas funcionalidades bem exclusivas, o jogo pode ser jogado de forma individual ou contra um amigo (2) jogadores. Resolvemos implementar algumas ideias como poder usar superpoderes, podendo o jogador conseguir arremessar até 3 (três) bolas contra o oponente tornando assim o jogo mais competitivo e com uma dificuldade maior imposta e como defesa temos uma outra função a de aumento da barra, assim podendo diminuir o espaço e ter uma maior chance de rebater o oponente.
                </v-card-text>
               
              </v-expansion-panel-content>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-row>
        </v-card>
      <v-card class="mt-5 ml-3 mr-3" >
        <v-row justify="center">
          <v-expansion-panels accordion>
            <v-expansion-panel>
              <v-expansion-panel-header><v-toolbar-title>Ideias do projeto</v-toolbar-title> </v-expansion-panel-header>
              <v-expansion-panel-content>
                <v-card-title>
                  IDEIAS USADAS
                </v-card-title>
                <v-card-text>
                  Usamos o tema do mortal kombat, Como gráfico do jogo usamos um visual um pouco tenebroso, usando assim caveiras e um ambiente escuro, por outro lado pra não ser deixado a magia da diversão do jogo, usamos imagens de algumas pessoas do grupo e até nossos professores trazendo assim também um aspecto mais divertido.
                </v-card-text>
                <v-card-title>
                  IDEIAS DESCARTADAS
                </v-card-title>
                <v-card-text>
                  Tinha como tema abordar uma campanha contra bullying e o uso de bebidas alcoólicas.
                </v-card-text>
              <v-card-title>Tecnologia usada</v-card-title>
              <v-card-text>Linguagem python</v-card-text>
              <v-card-text>Biblioteca PyGames</v-card-text>
              </v-expansion-panel-content>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-row>
        </v-card>
      <v-card class="mt-5 ml-3 mr-3" >
        <v-row justify="center">
          <v-expansion-panels accordion>
            <v-expansion-panel>
              <v-expansion-panel-header><v-toolbar-title>Conclusão</v-toolbar-title> </v-expansion-panel-header>
              <v-expansion-panel-content>
          
                <v-card-text>
                  Concluímos que o nosso projeto foi de grande aprendizagem para nossa equipe as ideias impostas conseguiriam ser executadas como planejado. A ideia pode ser continuada como com melhorias e novas funcionalidades para o jogo continuar atualizado.  
                </v-card-text>
               
              </v-expansion-panel-content>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-row>
        </v-card>
      </v-card>
      </v-col>
     
    </div>

</template>

<script>
  import router from '@/router';
  export default {
  data(){return {}}
  }
</script>
