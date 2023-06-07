<template>
    <div>
    <v-container>
    <v-card class="mt-5 ml-3 mr-3" >
    <v-row justify="center">
      <v-expansion-panels accordion>
        <v-expansion-panel>
          <v-expansion-panel-header><v-toolbar-title>Frame Menu</v-toolbar-title> </v-expansion-panel-header>
          <v-expansion-panel-content>
            <v-card>
              <v-responsive :aspect-ratio="16/9">
              <v-img contain  src="../assets/classe_freme_menu.png"></v-img>
              </v-responsive>
            </v-card>
            <v-card-title>
                Essa classe chamada Frame é usada para animar uma sequência de quadros (frames) em um jogo utilizando a biblioteca pygame.

                Aqui está uma explicação passo a passo do que a classe faz:
            </v-card-title>
            <v-card-subtitle>
              <v-card-subtitle>
                O construtor (__init__) inicializa o objeto Frame. Ele herda da classe pygame.sprite.Sprite para permitir que o objeto seja usado como um sprite em um grupo de sprites.                
              </v-card-subtitle>
              <v-card-subtitle>
                No construtor, a lista self.sprites é criada. É um atributo que armazena os quadros (frames) da animação do jogo. A classe carrega 24 imagens sequenciais com base na convenção de nomenclatura dos arquivos (por exemplo, pong_frames1.png, pong_frames2.png, ..., pong_frames24.png). Cada imagem é carregada usando a função pygame.image.load() e adicionada à lista self.sprites.
              </v-card-subtitle>
              <v-card-subtitle>
                self.atual é uma variável que armazena o índice atual da imagem que está sendo exibida na animação. Inicialmente, é definida como 0, o que significa que a primeira imagem na lista self.sprites será exibida.
              </v-card-subtitle>
              <v-card-subtitle>
                self.image é o atributo que representa a imagem atual que será exibida. É inicializado com a primeira imagem na lista self.sprites.
              </v-card-subtitle>
              <v-card-subtitle>
                self.rect é um retângulo que envolve a imagem atual. Ele é obtido usando o método get_rect() da imagem e, em seguida, definido para a posição (0, 0) no canto superior esquerdo.
              </v-card-subtitle>
              <v-card-subtitle>
                self.animar é uma variável booleana que controla se a animação está em andamento. Inicialmente, é definida como False, o que significa que a animação não está ocorrendo.
              </v-card-subtitle>
              <v-card-subtitle>
                O método AnimarFrame() é usado para iniciar a animação. Quando chamado, ele define self.animar como True, indicando que a animação deve começar.
              </v-card-subtitle>
              <v-card-subtitle>
                O método update() é chamado a cada quadro do jogo para atualizar o estado da animação. Se self.animar for True, a variável self.atual é incrementada em 0.1. Isso permite uma animação suave, avançando gradualmente para os quadros seguintes.
              </v-card-subtitle>
              <v-card-subtitle>
                Se self.atual for maior ou igual ao comprimento da lista self.sprites, significa que a animação chegou ao fim. Nesse caso, self.atual é definida como o último índice da lista (len(self.sprites) - 1) e self.animar é definida como False para interromper a animação.
              </v-card-subtitle>
              <v-card-subtitle>
                A imagem atual é atualizada para a imagem correspondente ao índice int(self.atual) na lista self.sprites. Isso altera a imagem exibida a cada quadro, criando a ilusão de animação.
              </v-card-subtitle>
            </v-card-subtitle>
            <v-card-title>
                Em resumo, essa classe permite carregar e exibir uma sequência de quadros (frames) em um jogo usando a biblioteca pygame, além de fornecer métodos para iniciar e controlar a animação.
            </v-card-title>
          </v-expansion-panel-content>
        </v-expansion-panel>
      </v-expansion-panels>
    </v-row>
    </v-card>
    <v-card class="mt-5 ml-3 mr-3" >
    <v-row justify="center">
      <v-expansion-panels accordion>
        <v-expansion-panel>
          <v-expansion-panel-header><v-toolbar-title>Game Over</v-toolbar-title> </v-expansion-panel-header>
          <v-expansion-panel-content>
            <v-card>
              <v-responsive :aspect-ratio="16/9">
              <v-img contain  src="../assets/class_gameover.png"></v-img>
              </v-responsive>
            </v-card>
            <v-card-title>
              Essa classe chamada GameOver é uma cena do jogo que é exibida quando o jogo termina. Ela herda da classe Scene, indicando que faz parte de um sistema de gerenciamento de cenas de jogo.

              O construtor __init__ dessa classe recebe dois parâmetros: head e winer (provavelmente um erro de digitação, deveria ser winner). A função super().__init__() é chamada para chamar o construtor da classe pai (Scene).

              Dentro do construtor, há várias inicializações de atributos. Aqui estão alguns dos atributos e suas respectivas inicializações:
            </v-card-title>
            <v-card-subtitle>
              <v-card-subtitle>
                self.vict: É atribuído o valor de self.victory. Pode ser uma variável ou método de outra parte do código que não foi mostrado.
              </v-card-subtitle>
              <v-card-subtitle>
                self.win: Recebe o valor do parâmetro winner
              </v-card-subtitle>
              <v-card-subtitle>
                self.Head: Recebe o valor do parâmetro head.
              </v-card-subtitle>
              <v-card-subtitle>
                self.Head_2: Recebe o próprio valor de self.Head_2, o que não faz muito sentido.
              </v-card-subtitle>
              <v-card-subtitle>
                self.bg: É criado um objeto Obj (que provavelmente representa um objeto gráfico) com a imagem 'GAME_OVER_FINALIZADO.jpg' e posição (0, 0). O objeto é adicionado a uma lista chamada self.all_sprites.
              </v-card-subtitle>
              <v-card-subtitle>
                self.trofel: É criado um objeto Obj com a imagem 'TROFEU.png' e posição (545, 190). Também é adicionado a self.all_sprites.
              </v-card-subtitle>
              <v-card-subtitle>
                self.text: É criado um objeto Text (provavelmente um objeto de texto) com uma fonte 'Retro_Gaming.ttf', tamanho de 40 pixels, texto self.win, cor branca e posição (30, 150).
              </v-card-subtitle>
              <v-card-subtitle>
                self.btn_menu: É criado um objeto Button (provavelmente um botão) com a imagem btn_game, posição (490, 660), rótulo 'MENU' e uma função self.back_menu associada ao evento de clique.
              </v-card-subtitle>
              <v-card-subtitle>
                self.head_Win(): É chamado o método head_Win, que define um objeto Obj para self.Head com base no valor de self.Head.
              </v-card-subtitle>
              <v-card-title>
                A classe GameOver também possui os seguintes métodos:
              </v-card-title>
              <v-card-subtitle>
                head_Win(): Verifica o valor de self.Head e cria um objeto Obj correspondente com base nesse valor. Os objetos são adicionados a self.all_sprites.
              </v-card-subtitle>
              <v-card-subtitle>
                back_menu(): Define a variável self.Menu como False
              </v-card-subtitle>
              <v-card-subtitle>
                events(event): Recebe um evento e repassa para o método events de self.btn_menu.
              </v-card-subtitle>
              <v-card-subtitle>
                update(): Chama o método draw de self.text, self.head_Win() e self.btn_menu.draw(). Em seguida, chama o método update da classe pai (super().update()) e retorna o resultado.
              </v-card-subtitle>
             

            </v-card-subtitle> 
            <v-card-title>
              No geral, a classe GameOver parece ser responsável por exibir a cena de fim de jogo, exibindo uma imagem de fundo, um troféu, um texto de vitória, uma imagem do vencedor e um botão de menu.
            </v-card-title>
          </v-expansion-panel-content>
        </v-expansion-panel>
      </v-expansion-panels>
    </v-row>
    </v-card>
    <v-card class="mt-5 ml-3 mr-3" >
    <v-row justify="center">
      <v-expansion-panels accordion>
        <v-expansion-panel>
          <v-expansion-panel-header><v-toolbar-title>Pong Game</v-toolbar-title> </v-expansion-panel-header>
          <v-expansion-panel-content>
            <v-card>
              <v-responsive :aspect-ratio="16/9">
              <v-img contain  src="../assets/class_pong.png"></v-img>
              </v-responsive>
            </v-card>
            <v-card-title>
              Essa classe, chamada PongGame, representa a cena principal do jogo Pong. Ela herda da classe Scene, indicando que é uma cena do jogo. Aqui estão as principais funcionalidades da classe:
            </v-card-title>
            <v-card-subtitle>
              <v-card-subtitle>
                No método __init__, são inicializados todos os elementos do jogo, como a música, as imagens de fundo, a bola, as barras dos jogadores, a vida dos jogadores, os textos e os jogadores.
              </v-card-subtitle>
              <v-card-subtitle>
                Os métodos life_player1 e life_player2 são responsáveis por atualizar a barra de vida dos jogadores, de acordo com o impacto da bola.
              </v-card-subtitle>
              <v-card-subtitle>
                Os métodos colidSuperPl1 e colidSuperPl2 lidam com as colisões entre a bola e as barras dos jogadores, fazendo com que a bola mude de direção e causando efeitos sonoros.
              </v-card-subtitle>
              <v-card-subtitle>
                O método spawBall controla o movimento da bola e verifica se ela colide com as bordas do campo, atualizando a pontuação dos jogadores.
              </v-card-subtitle>
              <v-card-subtitle>
                O método colisionBall verifica se a bola colide com as barras dos jogadores, alterando sua direção e tocando um efeito sonoro.
              </v-card-subtitle>
              <v-card-subtitle>
                O método limiBall verifica se a bola atinge os limites superior e inferior do campo, invertendo sua direção e reproduzindo um efeito sonoro.
              </v-card-subtitle>
              <v-card-subtitle>
                O método limitPlay limita o movimento dos jogadores dentro do campo.
              </v-card-subtitle>
              <v-card-subtitle>
                O método update atualiza todos os elementos do jogo, incluindo a entrada do jogador, o movimento dos jogadores, a atualização da corda, a verificação de colisões, o movimento e a colisão da bola, e a atualização da exibição.
              </v-card-subtitle>
              <v-card-subtitle>
                O método events é responsável por lidar com eventos de entrada, como pressionar teclas.
              </v-card-subtitle>
             
            </v-card-subtitle>
            <v-card-title>
              Essa classe representa a lógica principal do jogo Pong, controlando todos os elementos e interações durante o jogo.
            </v-card-title>
          </v-expansion-panel-content>
        </v-expansion-panel>
      </v-expansion-panels>
    </v-row>
    </v-card>
    <v-card class="mt-5 ml-3 mr-3" >
    <v-row justify="center">
      <v-expansion-panels accordion>
        <v-expansion-panel>
          <v-expansion-panel-header><v-toolbar-title>Pong Menu</v-toolbar-title> </v-expansion-panel-header>
          <v-expansion-panel-content>
            <v-card>
              <v-responsive :aspect-ratio="16/9">
              <v-img contain  src="../assets/class_pongmenu.png"></v-img>
              </v-responsive>
            </v-card>
            <v-card-title>
              Essa classe, chamada PongMenu, representa o menu do jogo Pong. Ela herda da classe Scene, indicando que é uma cena do jogo.
            </v-card-title>
            <v-card-subtitle>

              <v-card-subtitle>
                No método __init__, algumas inicializações são feitas. O atributo self.bg é um objeto que representa a imagem de fundo do menu. Os atributos self.btn_player2, self.Gerhard, self.messias, self.lucas, self.pierre, self.rafael, self.sandro e self.leandro são todos objetos de diferentes elementos do menu, como botões e imagens de personagens. 
              </v-card-subtitle>
              <v-card-subtitle>
                No método update, a lógica de atualização do menu é implementada. Se o menu_frame não está animando, o botão self.btn_player2 é desenhado na tela. Caso contrário, o frame_sprites é atualizado.              
              </v-card-subtitle>
              <v-card-subtitle>
                Os métodos nextScenePL2 e nextScenePL1 são chamados quando o botão self.btn_player2 é clicado. Eles reproduzem um som e animam o menu_frame, adicionando-o ao frame_sprites. Além disso, eles definem o atributo verificar_pl2 ou verificar_pl1 como True.              
              </v-card-subtitle>
              <v-card-subtitle>
                No método events, várias interações do mouse são tratadas. O método events é chamado quando ocorrem eventos no jogo, como cliques do mouse. Por exemplo, quando o botão esquerdo do mouse é clicado, verifica-se se a posição do clique colide com as imagens dos personagens Gerhard, messias, lucas, pierre, rafael, sandro e leandro. Dependendo da colisão, diferentes ações são realizadas, como reprodução de música e definição do atributo Head.             
              </v-card-subtitle>
             
            </v-card-subtitle>
            <v-card-title>
              No geral, a classe PongMenu é responsável por gerenciar o menu do jogo Pong, incluindo a exibição dos elementos do menu, interações do mouse e transições para outras cenas do jogo.           
            </v-card-title>
          </v-expansion-panel-content>
        </v-expansion-panel>
      </v-expansion-panels>
    </v-row>
    </v-card>
    <v-card class="mt-5 ml-3 mr-3" >
    <v-row justify="center">
      <v-expansion-panels accordion>
        <v-expansion-panel>
          <v-expansion-panel-header><v-toolbar-title>Player 1</v-toolbar-title> </v-expansion-panel-header>
          <v-expansion-panel-content>
            <v-card>
              <v-responsive :aspect-ratio="16/9">
              <v-img contain  src="../assets/class_player_1.png"></v-img>
              </v-responsive>
            </v-card>
            <v-card-title>
              Essa classe, chamada Player1, representa o jogador 1 no jogo Pong. Ela herda da classe Obj, indicando que é um objeto do jogo.
            </v-card-title>
            <v-card-subtitle>
              <v-card-subtitle>
                No método __init__, algumas inicializações são feitas. O método super().__init__(img, pos, *group) é chamado para inicializar o objeto com uma imagem, posição e grupos aos quais pertence. O atributo self.direction é um vetor de direção que armazena as direções em que o jogador está se movendo. O atributo self.head armazena a rotação da cabeça do jogador. O atributo self.speed define a velocidade de movimento do jogador. O atributo self.shots1 é um grupo de sprites que armazena os tiros disparados pelo jogador. Os atributos self.tics, self.time_oso, self.tics_2 e self.verif são usados para controlar o tempo e as ações do jogador.              </v-card-subtitle>
              <v-card-subtitle>
                No método input, é tratada a entrada do jogador através do teclado. Dependendo das teclas pressionadas, as direções x e y são atualizadas. Se a tecla de espaço for pressionada, é realizado um controle de tempo para permitir que o jogador dispare uma bola. O método showHead é chamado para criar uma nova bola de tiro, dependendo da cabeça do jogador selecionada.
              </v-card-subtitle>
              <v-card-subtitle>
                O método move é responsável por atualizar a posição do jogador com base na direção e velocidade definidas.
              </v-card-subtitle>
              <v-card-subtitle>
                O método update chama os métodos move e input para atualizar o jogador a cada quadro.
              </v-card-subtitle>
              <v-card-subtitle>
                A segunda classe, chamada ShotBallPl1, representa as bolas de tiro disparadas pelo jogador 1. Ela também herda da classe Obj.
              </v-card-subtitle>
              <v-card-subtitle>
                No método __init__, o método super().__init__(img, pos, *group) é chamado para inicializar o objeto com uma imagem, posição e grupos aos quais pertence. O atributo self.speed_x representa a velocidade horizontal da bola de tiro. O atributo self.speed_y representa a velocidade vertical da bola de tiro. O atributo self.pl1 armazena uma referência ao jogador 1.
              </v-card-subtitle>
              <v-card-subtitle>
                No método update, a posição da bola de tiro é atualizada de acordo com as velocidades horizontais e verticais.
              </v-card-subtitle>
             </v-card-subtitle>
          </v-expansion-panel-content>
        </v-expansion-panel>
      </v-expansion-panels>
    </v-row>
    </v-card>
    <v-card class="mt-5 ml-3 mr-3" >
    <v-row justify="center">
      <v-expansion-panels accordion>
        <v-expansion-panel>
          <v-expansion-panel-header><v-toolbar-title>Player 2</v-toolbar-title> </v-expansion-panel-header>
          <v-expansion-panel-content>
            <v-card>
              <v-responsive :aspect-ratio="16/9">
              <v-img contain  src="../assets/class_player_2.png"></v-img>
              </v-responsive>
            </v-card>
            <v-card-title>
              Essa classe, chamada Player2, representa o jogador 2 no jogo Pong. Ela também herda da classe Obj, indicando que é um objeto do jogo.
            </v-card-title>
            <v-card-subtitle>
              <v-card-subtitle>
                No método __init__, são feitas algumas inicializações. O método super().__init__(img, pos, *group) é chamado para inicializar o objeto com uma imagem, posição e grupos aos quais pertence. O atributo self.direction é um vetor de direção que armazena as direções em que o jogador está se movendo. O atributo self.head armazena a rotação da cabeça do jogador. O atributo self.speed define a velocidade de movimento do jogador. O atributo self.shots2 é um grupo de sprites que armazena os tiros disparados pelo jogador. Os atributos self.tics, self.time_oso, self.tics_2 e self.verif são usados para controlar o tempo e as ações do jogador.
              </v-card-subtitle>
              <v-card-subtitle>
                No método input, é tratada a entrada do jogador através do teclado. Dependendo das teclas pressionadas, as direções x e y são atualizadas. Se a tecla "1" do teclado numérico for pressionada, é realizado um controle de tempo para permitir que o jogador dispare uma bola. O método showHead é chamado para criar uma nova bola de tiro, dependendo da cabeça do jogador selecionada.
              </v-card-subtitle>
              <v-card-subtitle>
                O método move é responsável por atualizar a posição do jogador com base na direção e velocidade definidas.
              </v-card-subtitle>
              <v-card-subtitle>
                O método update chama os métodos move e input para atualizar o jogador a cada quadro.
              </v-card-subtitle>
              <v-card-subtitle>
                A segunda classe, chamada ShotBallPl2, representa as bolas de tiro disparadas pelo jogador 2. Ela também herda da classe Obj.
              </v-card-subtitle>
              <v-card-subtitle>
                No método __init__, o método super().__init__(img, pos, *group) é chamado para inicializar o objeto com uma imagem, posição e grupos aos quais pertence. O atributo self.speed_x representa a velocidade horizontal da bola de tiro. O atributo self.speed_y representa a velocidade vertical da bola de tiro. O atributo self.pl2 armazena uma referência ao jogador 2.
              </v-card-subtitle>
              <v-card-subtitle>
                No método update, a posição da bola de tiro é atualizada de acordo com as velocidades horizontais e verticais.
            
               </v-card-subtitle>
              </v-card-subtitle> 
          </v-expansion-panel-content>
        </v-expansion-panel>
      </v-expansion-panels>
    </v-row>
    </v-card>
    </v-container>
    </div>
</template>
<script>
export default {

}

</script>