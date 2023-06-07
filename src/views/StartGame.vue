<template>
    <div>
    <v-container >
    <v-card class="mt-5 ml-3 mr-3" >
    <v-row justify="center">
      <v-expansion-panels accordion>
        <v-expansion-panel>
          <v-expansion-panel-header><v-toolbar-title>Start Game</v-toolbar-title> </v-expansion-panel-header>
          <v-expansion-panel-content>
            <v-card>
              <v-responsive :aspect-ratio="16/9">
              <v-img contain  src="../assets/classe_startgame.png"></v-img>
              </v-responsive>
            </v-card>
            <v-card-title>
              Essa classe representa o controle principal do jogo Pong. Vamos analisar o que cada parte do código faz:
            </v-card-title>
            <v-card-subtitle>
              <v-card-subtitle>
              A classe StartGame é inicializada com a configuração do Pygame, incluindo a inicialização dos módulos Pygame para gráficos, som e fontes.
                
              </v-card-subtitle>
              <v-card-subtitle>
              A tela do jogo é criada com as dimensões especificadas em WIDTH e HEIGHT.
                
              </v-card-subtitle>
              <v-card-subtitle>
              O jogo começa no menu principal do Pong (PongMenu()).
                
              </v-card-subtitle>
              <v-card-subtitle>
              O método run é responsável pelo loop principal do jogo. Ele captura eventos do Pygame, atualiza a cena atual, desenha a cena na tela e atualiza a exibição. O loop continua até que o jogo seja encerrado.
                
              </v-card-subtitle>
              <v-card-subtitle>
              O método selecPong é chamado a cada iteração do loop principal. Ele verifica o estado da cena atual e toma decisões com base nesse estado.
                
              </v-card-subtitle>
              <v-card-subtitle>
              Se o jogador 1 não estiver selecionado, a cena é alterada para o modo de jogador vs. computador (Player2_bot) com as cabeças (head e head2) escolhidas.
                
              </v-card-subtitle>
              <v-card-subtitle>
              Se o jogador 2 não estiver selecionado, a música de introdução é interrompida e a cena é alterada para o jogo principal (PongGame) com as cabeças escolhidas.
                
              </v-card-subtitle>
              <v-card-subtitle>
              Se o jogador 1 tiver atingido 0 pontos, a cena é alterada para a tela de fim de jogo (GameOver) com a cabeça do jogador 2 e o texto indicando que o "Player2" venceu.
                
              </v-card-subtitle>
              <v-card-subtitle>
              Se o jogador 2 tiver atingido 0 pontos, a cena é alterada para a tela de fim de jogo com a cabeça do jogador 1 e o texto indicando que o "Player1" venceu.
                
              </v-card-subtitle>
              <v-card-subtitle>
              Se o menu principal não estiver ativo, a cena é alterada para o menu principal do Pong.
                
              </v-card-subtitle>
            </v-card-subtitle>
            <v-card-title>
              Em resumo, a classe StartGame gerencia a execução do jogo Pong, controlando a transição entre diferentes cenas (menu, jogo, tela de fim de jogo) com base em eventos e estados específicos.
            </v-card-title>
          </v-expansion-panel-content>
        </v-expansion-panel>
      </v-expansion-panels>
    </v-row>
    </v-card>
    <v-card class="mt-5 ml-3 mr-3">
    <v-row justify="center">
      <v-expansion-panels accordion>
        <v-expansion-panel>
          <v-expansion-panel-header><v-toolbar-title>Setings</v-toolbar-title> </v-expansion-panel-header>
          <v-expansion-panel-content>
            <v-card>
              <v-responsive :aspect-ratio="16/9">
              <v-img contain src="../assets/classe_setings.png"></v-img>
              </v-responsive>
            </v-card>
            <v-card-title>
              Essa parte do código define algumas constantes e caminhos de arquivos utilizados em um jogo ou aplicação que parece ser relacionado ao Pong. Vamos analisar o significado de cada linha:
            </v-card-title>
            <v-card-text>
              <v-card-text>
              WIDTH = 1280: Define a largura da tela do jogo ou aplicação como 1280 pixels.
                
              </v-card-text>
              <v-card-text>

              HEIGHT = 720: Define a altura da tela do jogo ou aplicação como 720 pixels.
              </v-card-text>
              <v-card-text>
              main_menu = 'assets/main_menu/': Define o diretório onde estão localizados os arquivos relacionados ao menu principal do jogo ou aplicação.

              </v-card-text>
              <v-card-text>
              sonds = 'assets/assets_pong/songs/': Define o diretório onde estão localizados os arquivos de músicas e sons utilizados no jogo ou aplicação.

              </v-card-text>
              <v-card-text>
              pong_images = 'assets/assets_pong/image/': Define o diretório onde estão localizadas as imagens utilizadas no jogo ou aplicação.

              </v-card-text>
              <v-card-text>
              pong_heads = 'assets/assets_pong/image/heads/': Define o diretório onde estão localizadas as imagens relacionadas às cabeças (sprites) utilizadas no jogo ou aplicação.

              </v-card-text>
              <v-card-text>
              pong_fonts = 'assets/assets_pong/fonts/': Define o diretório onde estão localizadas as fontes de texto utilizadas no jogo ou aplicação.

              </v-card-text>
              <v-card-text>
              pong_cenario = 'assets/assets_pong/image/cenario/': Define o diretório onde estão localizadas as imagens relacionadas ao cenário do jogo ou aplicação.

              </v-card-text>
              <v-card-text>
              pong_frames = 'assets/assets_pong/FRAMES_MENU/': Define o diretório onde estão localizadas as imagens dos quadros (frames) utilizados no menu do jogo ou aplicação.

              </v-card-text>
              <v-card-text>
              pong_balls = 'assets/assets_pong/image/heads/balls/': Define o diretório onde estão localizadas as imagens relacionadas às bolas utilizadas no jogo ou aplicação.

              </v-card-text>
              <v-card-text>
              primary_color = [255, 255, 255]: Define a cor primária utilizada no jogo ou aplicação como branco (RGB: 255, 255, 255).

              </v-card-text>
              <v-card-text>
              secundary_color = [86, 64, 166, 255]: Define a cor secundária utilizada no jogo ou aplicação como um tom de roxo (RGB: 86, 64, 166, 255).

              </v-card-text>
              <v-card-text>
              yellow = [254, 201, 41, 255]: Define a cor amarela utilizada no jogo ou aplicação (RGB: 254, 201, 41, 255).

              </v-card-text>
              <v-card-text>
              btn_game = [169,143,133,255]: Define a cor de um botão específico do jogo ou aplicação (RGB: 169, 143, 133, 255).

              </v-card-text>
            </v-card-text>
            <v-card-text>
              Essas constantes e caminhos de arquivos são usados posteriormente no código para carregar imagens, sons e definir cores em diferentes partes do jogo ou aplicação.
            </v-card-text>
          </v-expansion-panel-content>
        </v-expansion-panel>
      </v-expansion-panels>
    </v-row>
    </v-card>
    <v-card class="mt-5 ml-3 mr-3">
    <v-row justify="center">
      <v-expansion-panels accordion>
        <v-expansion-panel>
          <v-expansion-panel-header><v-toolbar-title>Scene</v-toolbar-title> </v-expansion-panel-header>
          <v-expansion-panel-content>
            <v-img src="../assets/classe_scene.png"></v-img>
            <v-card-title>
              A classe Scene parece ser uma classe base para uma cena em um jogo ou aplicação desenvolvida com Pygame. A classe possui métodos para lidar com eventos, desenhar e atualizar elementos na tela. Vamos analisar o que cada parte dessa classe faz:
            </v-card-title>
            <v-card-subtitle>
              <v-card-subtitle>
              def __init__(self): O construtor da classe Scene é responsável por inicializar os atributos e configurações iniciais da cena.
                
              </v-card-subtitle>
              <v-card-subtitle>
              pygame.display.set_caption("teste Obj"): Define o título da janela do Pygame como "teste Obj".

              </v-card-subtitle>
              <v-card-subtitle>
              self.display = pygame.display.get_surface(): Retorna a superfície atual associada à janela principal do Pygame. Essa superfície é armazenada no atributo self.display e será usada posteriormente para desenhar elementos.

              </v-card-subtitle>
              <v-card-subtitle>
              self.all_sprites = pygame.sprite.Group(): Cria um grupo de sprites chamado self.all_sprites. Esse grupo é usado para armazenar e gerenciar vários sprites que serão desenhados e atualizados na cena.

              </v-card-subtitle>
              <v-card-subtitle>
              A partir da linha 9 até a linha 22, diversos sons são carregados usando pygame.mixer.Sound(). Esses sons parecem ser efeitos sonoros e músicas que podem ser reproduzidos durante o jogo ou a cena.

              </v-card-subtitle>
              <v-card-subtitle>
              self.Game = True, self.Menu = True, self.active = True, self.player_1 = True, self.player_2 = True: Esses atributos parecem ser variáveis de controle do estado do jogo ou da cena.

              </v-card-subtitle>
              <v-card-subtitle>
              self.ponto_1 = 300, self.ponto_2 = 300: Atribui um valor inicial de pontos para os jogadores 1 e 2.

              </v-card-subtitle>
              <v-card-subtitle>
              self.Head = '', self.Head_2 = '': Atribui uma string vazia para as variáveis self.Head e self.Head_2.

              </v-card-subtitle>
              <v-card-subtitle>
              self.fade = Fade(1): Cria uma instância da classe Fade com um valor de velocidade de transição (fade) igual a 1.

              </v-card-subtitle>
              <v-card-subtitle>
              def events(self, event): O método events é chamado para lidar com eventos relacionados à cena. Neste caso, o método está vazio, então não realiza nenhuma ação específica.

              </v-card-subtitle>
              <v-card-subtitle>
              def draw(self): O método draw é responsável por desenhar os elementos da cena na tela. Neste caso, ele chama o método draw do grupo de sprites self.all_sprites para desenhar os sprites na superfície self.display.

              </v-card-subtitle>
              <v-card-subtitle>
              def update(self): O método update é responsável por atualizar os elementos da cena. Neste caso, ele chama o método update do grupo de sprites self.all_sprites para atualizar os sprites.

              </v-card-subtitle>
             
            </v-card-subtitle>
            <v-card-title>
              A classe Fade é uma classe separada e parece ser usada para criar um efeito de desvanecimento na tela. Ela possui um atributo de alfa (self.alpha) que controla a transparência de uma superfície preta que é desenhada na tela. O método draw é responsável por reduzir gradualmente o valor de alfa para criar o efeito de desvanecimento.

              Essas classes podem ser usadas como base para criar cenas e efeitos visuais em um jogo ou aplicação usando o Pygame.
            </v-card-title>
          </v-expansion-panel-content>
        </v-expansion-panel>
      </v-expansion-panels>
    </v-row>
    </v-card>
    <v-card class="mt-5 ml-3 mr-3">
    <v-row justify="center">
      <v-expansion-panels accordion>
        <v-expansion-panel>
          <v-expansion-panel-header><v-toolbar-title>Text</v-toolbar-title> </v-expansion-panel-header>
          <v-expansion-panel-content>
            <v-card>
              <v-responsive :aspect-ratio="16/9">
              <v-img contain src="../assets/classe_text.png"></v-img>
              </v-responsive>
            </v-card>
            <v-card-title>
              classe para renderizar e exibir texto na tela usando o Pygame. Vamos analisar o que cada parte dessa classe faz:
            </v-card-title>
            <v-card-subtitle>
              <v-card-subtitle>
              def __init__(self, font, size, text, color, pos): O construtor da classe Text é responsável por inicializar os atributos e configurações iniciais do texto.
                
              </v-card-subtitle>
              <v-card-subtitle>
              self.display = pygame.display.get_surface(): Retorna a superfície atual associada à janela principal do Pygame. Essa superfície é armazenada no atributo self.display e será usada posteriormente para desenhar o texto.

              </v-card-subtitle>
              <v-card-subtitle>
              self.font = pygame.font.Font(font, size): Cria um objeto de fonte com base no arquivo de fonte especificado e no tamanho da fonte.

              </v-card-subtitle>
              <v-card-subtitle>
              self.text = self.font.render(text, True, color): Renderiza o texto usando a fonte e o tamanho definidos, com a cor especificada. O resultado é armazenado no atributo self.text como uma superfície de texto renderizada.

              </v-card-subtitle>
             
              <v-card-subtitle>
              self.text_rect = self.text.get_rect(center=pos): Obtém o retângulo que envolve o texto renderizado e o posiciona no centro com base nas coordenadas especificadas em pos.

              </v-card-subtitle>
              <v-card-subtitle>
              self.color = color: Armazena a cor do texto.

              </v-card-subtitle>
              <v-card-subtitle>
              self.position = pos: Armazena a posição do texto.

              </v-card-subtitle>
              <v-card-subtitle>
              self.text_alpha = 255: Armazena o valor inicial da transparência do texto (alfa).

              </v-card-subtitle>
              <v-card-subtitle>
              self.alpha_speed = 5: Armazena a velocidade de alteração da transparência do texto.

              </v-card-subtitle>
              <v-card-subtitle>
              def draw(self): O método draw é responsável por desenhar o texto na tela. Ele usa o método blit para desenhar a superfície de texto (self.text) na superfície de exibição (self.display), na posição especificada (self.position).

              </v-card-subtitle>
              <v-card-subtitle>
              def draw_center(self): O método draw_center é semelhante ao método draw, mas em vez de usar a posição específica, ele usa o retângulo do texto (self.text_rect) para centralizar o texto na tela.

              </v-card-subtitle>
              <v-card-subtitle>
              def text_update(self, text, color): O método text_update atualiza o texto e sua cor. Ele recebe o novo texto e a nova cor como parâmetros, renderiza o novo texto usando a nova cor e atualiza o atributo self.text com a nova superfície de texto renderizada.

              </v-card-subtitle>
             
            </v-card-subtitle>
            <v-card-title>
              Essa classe Text é útil para renderizar e exibir texto na tela em um jogo ou aplicação usando o Pygame. Ela permite controlar a fonte, o tamanho, a cor e a posição do texto, além de oferecer métodos para desenhar o texto de forma centralizada e atualizá-lo com novos valores.
            </v-card-title>
           
           
          </v-expansion-panel-content>
        </v-expansion-panel>
      </v-expansion-panels>
    </v-row>
  </v-card>
    <v-card class="mt-5 ml-3 mr-3">
    <v-row justify="center">
      <v-expansion-panels accordion>
        <v-expansion-panel>
          <v-expansion-panel-header> <v-toolbar-title>Object</v-toolbar-title></v-expansion-panel-header>
          <v-expansion-panel-content>
            <v-card>
              <v-card>
                <v-responsive :aspect-ratio="16/9">
                <v-img contain src="../assets/Obj_class.png"></v-img>
                </v-responsive>
              </v-card>
              <v-card-title>
                A classe Obj é uma subclasse da classe pygame.sprite.Sprite no Pygame. Ela é usada para criar objetos gráficos que podem ser exibidos e manipulados em um jogo ou aplicação.

                A classe pygame.sprite.Sprite é uma classe base fornecida pelo Pygame que facilita a criação e manipulação de sprites. Um sprite é uma entidade gráfica que pode ser exibida na tela, geralmente representando um personagem, objeto ou elemento interativo no jogo.

                A classe Obj tem um construtor __init__() que inicializa os atributos do objeto. Vamos analisar o que cada linha do construtor faz:
              </v-card-title>

              <v-card-subtitle>
                <v-card-subtitle>
                super().__init__(*groups): Chama o construtor da classe pai pygame.sprite.Sprite, inicializando a instância do objeto como um sprite.
                  
                </v-card-subtitle>
                <v-card-subtitle>
                self.image = pygame.image.load(img): Carrega uma imagem do arquivo especificado por img e atribui a imagem carregada ao atributo self.image. Isso define a aparência gráfica do objeto.

                </v-card-subtitle>
                <v-card-subtitle>
                if size: self.image = pygame.transform.scale(self.image, size): Verifica se foi fornecido um tamanho (size) para o objeto. Se sim, redimensiona a imagem do objeto para esse tamanho usando a função pygame.transform.scale(). Isso permite ajustar o tamanho do objeto na tela.

                </v-card-subtitle>
                <v-card-subtitle>
                self.rect = self.image.get_rect(topleft=pos): Obtém o retângulo que envolve a imagem do objeto usando o método get_rect() da imagem. O argumento topleft=pos define a posição inicial do retângulo do objeto na tela, com base nas coordenadas especificadas em pos.

                </v-card-subtitle>
                <v-card-subtitle>
                self.frame = 0: Inicializa o atributo self.frame como zero. Este atributo pode ser usado para controlar a animação do objeto, se necessário.

                </v-card-subtitle>
                <v-card-subtitle>
                self.tic = 0: Inicializa o atributo self.tic como zero. Este atributo pode ser usado para controlar a lógica de temporização do objeto, se necessário.

                </v-card-subtitle>

              </v-card-subtitle>
              <v-card-title>
               Essa classe fornece uma estrutura básica para a criação de objetos gráficos usando imagens carregadas. Os objetos criados a partir dessa classe podem ser usados como sprites em jogos e manipulados dentro de grupos de sprites do Pygame, permitindo a detecção de colisões, animação e outras interações visuais.
              </v-card-title>
                <v-card>
                    <v-img contain src="../assets/Obj_class_obg_bg.png"></v-img>
                </v-card>
             
              <v-card-title>
                A classe ObjBg é outra subclasse da classe pygame.sprite.Sprite no Pygame. Ela é usada para criar objetos gráficos que funcionam como plano de fundo animado, alternando entre várias imagens.

                Vamos analisar o que cada parte dessa classe faz:
              </v-card-title>
              <v-card-subtitle>
                <v-card-subtitle>
                super().__init__(*groups): Chama o construtor da classe pai pygame.sprite.Sprite, inicializando a instância do objeto como um sprite.
                  
                </v-card-subtitle>
                <v-card-subtitle>
                self.images = [pygame.transform.scale(pygame.image.load(img), (1280, 720)) for img in images]: Carrega uma lista de imagens especificadas por images e redimensiona cada imagem para a largura de 1280 pixels e altura de 720 pixels usando pygame.transform.scale(). As imagens redimensionadas são armazenadas na lista self.images.

                </v-card-subtitle>
                <v-card-subtitle>
                self.image_index = 0: Inicializa o atributo self.image_index como zero. Ele controla o índice da imagem atual que está sendo exibida no plano de fundo.

                </v-card-subtitle>
                <v-card-subtitle>
                self.image = self.images[self.image_index]: Atribui a primeira imagem da lista self.images ao atributo self.image. Essa será a imagem inicial do plano de fundo.

                </v-card-subtitle>
                <v-card-subtitle>
                self.rect = self.image.get_rect(topleft=pos): Obtém o retângulo que envolve a imagem do plano de fundo usando o método get_rect() da imagem. O argumento topleft=pos define a posição inicial do retângulo do plano de fundo na tela, com base nas coordenadas especificadas em pos.

                </v-card-subtitle>
                <v-card-subtitle>
                self.frame = 0: Inicializa o atributo self.frame como zero. Este atributo pode ser usado para controlar a animação do plano de fundo, se necessário.

                </v-card-subtitle>
                <v-card-subtitle>
                self.tic = 0: Inicializa o atributo self.tic como zero. Este atributo pode ser usado para controlar a lógica de temporização do plano de fundo, se necessário.

                </v-card-subtitle>
                <v-card-subtitle>
                self.image_interval = 400: Define o intervalo de tempo (em unidades de lógica do jogo) entre as trocas de imagem do plano de fundo. Neste exemplo, a cada 400 unidades de tempo, o plano de fundo será atualizado para a próxima imagem.

                </v-card-subtitle>
                <v-card-subtitle>
                self.fade_duration = 30: Define a duração (em unidades de lógica do jogo) da transição de fade entre as imagens do plano de fundo. Neste exemplo, a transição de fade será concluída em 30 unidades de tempo.

                </v-card-subtitle>
                <v-card-subtitle>
                self.fade_alpha = 0: Inicializa o atributo self.fade_alpha como zero. Ele controla a opacidade do plano de fundo durante a transição de fade.

                </v-card-subtitle>
                <v-card-subtitle>
                def update(self): Este método é chamado a cada quadro do jogo para atualizar o estado do objeto de plano de fundo.

                </v-card-subtitle>
                <v-card-subtitle>
                self.tic += 1: Incrementa o contador de tempo self.tic em uma unidade.

                </v-card-subtitle>
                <v-card-subtitle>
                if self.tic >= self.image_interval:: Verifica se o contador de tempo self.tic alcançou ou excedeu o intervalo definido em self.image_interval.

                </v-card-subtitle>
                <v-card-subtitle>
                self.image_index = (self.image_index + 1) % len(self.images): Calcula o índice da próxima imagem no plano de fundo, permitindo que o plano de fundo alterne entre as imagens na lista self.images. O uso de % len(self.images) garante que o índice permaneça dentro dos limites da lista.

                </v-card-subtitle>
                <v-card-subtitle>
                self.image = self.images[self.image_index]: Atribui a próxima imagem do plano de fundo ao atributo self.image.

                </v-card-subtitle>
                <v-card-subtitle>
                self.fade_alpha = 0: Reinicia o valor de self.fade_alpha para zero, indicando o início de uma nova transição de fade.

                </v-card-subtitle>
                <v-card-subtitle>
                if self.fade_alpha &lt; 200:: Verifica se a opacidade do plano de fundo, self.fade_alpha, é menor que 200. Isso determina se a transição de fade está em andamento ou concluída.

                </v-card-subtitle>
                <v-card-subtitle>
                self.fade_alpha += int(200 / self.fade_duration): Incrementa o valor de self.fade_alpha com base na duração definida em self.fade_duration, fazendo com que a opacidade aumente gradualmente durante a transição de fade.

                </v-card-subtitle>
                <v-card-subtitle>
                self.image.set_alpha(self.fade_alpha): Define o valor de opacidade da imagem do plano de fundo usando o método set_alpha(). Isso ajusta a opacidade da imagem para que a transição de fade seja aplicada visualmente.

                </v-card-subtitle>
                
              </v-card-subtitle>
              <v-card-title>
                Essa classe permite a criação de um plano de fundo animado com transições suaves entre várias imagens. Cada imagem é exibida por um determinado intervalo de tempo, e durante a transição de uma imagem para outra, é aplicado um efeito de fade para tornar a mudança mais suave.
              </v-card-title>

          </v-card>
          </v-expansion-panel-content>
        </v-expansion-panel>
      </v-expansion-panels>
    </v-row>
  </v-card>
  <v-card class="mt-5 ml-3 mr-3">
    <v-row justify="center">
      <v-expansion-panels accordion>
        <v-expansion-panel>
          <v-expansion-panel-header><v-toolbar-title>Animation</v-toolbar-title> </v-expansion-panel-header>
          <v-expansion-panel-content>
            <v-img contain src="../assets/animation_class.png"></v-img>
            <v-card-title>
              A classe Animation é usada para animar uma imagem em um loop contínuo, reposicionando-a verticalmente em um cenário infinito. Ela usa a classe Obj para criar duas instâncias de objeto gráfico a partir de uma imagem fornecida.

              Vamos analisar o que cada parte dessa classe faz:
            </v-card-title>
            <v-card-subtitle>
              <v-card-subtitle>
              def __init__(self, img, pos1, pos2, *group): O construtor da classe Animation recebe uma imagem (img) e duas posições (pos1 e pos2) como argumentos, além de um grupo opcional. O construtor inicializa duas instâncias da classe Obj com a mesma imagem, mas em posições distintas.

              </v-card-subtitle>
              <v-card-subtitle>
              self.bg = Obj(img, pos1, *group): Cria uma instância da classe Obj chamada self.bg, usando a imagem fornecida (img) e a primeira posição (pos1). Essa instância representa a primeira imagem no loop da animação.

              </v-card-subtitle>
              <v-card-subtitle>
              self.bg2 = Obj(img, pos2, *group): Cria uma segunda instância da classe Obj chamada self.bg2, usando a mesma imagem (img) e a segunda posição (pos2). Essa instância representa a imagem seguinte no loop da animação.

              </v-card-subtitle>
              <v-card-subtitle>
              def updateCorda(self): O método updateCorda é responsável por atualizar a posição das duas imagens da animação. Ele move as imagens verticalmente incrementando suas coordenadas Y por um valor fixo (5 no exemplo fornecido).

              </v-card-subtitle>
              <v-card-subtitle>
              self.bg.rect.y += 5: Incrementa a coordenada Y da primeira imagem (self.bg) em 5 unidades.

              </v-card-subtitle>
              <v-card-subtitle>
              self.bg2.rect.y += 5: Incrementa a coordenada Y da segunda imagem (self.bg2) em 5 unidades.

              </v-card-subtitle>
              <v-card-subtitle>
              if self.bg.rect.y >= HEIGHT: self.bg.rect.y = 0 - HEIGHT: Verifica se a coordenada Y da primeira imagem (self.bg) atingiu ou ultrapassou o valor da altura (HEIGHT) da tela. Se sim, reposiciona a primeira imagem acima do topo da tela, para criar um efeito contínuo de loop vertical.

              </v-card-subtitle>
              <v-card-subtitle>
              if self.bg2.rect.y == HEIGHT: self.bg2.rect.y = - HEIGHT: Verifica se a coordenada Y da segunda imagem (self.bg2) é igual à altura (HEIGHT) da tela. Se sim, reposiciona a segunda imagem acima do topo da tela, para criar um efeito contínuo de loop vertical.

              </v-card-subtitle>
              

            </v-card-subtitle>
            <v-card-text>
              Essa classe é útil para criar animações de cenários infinitos, onde uma imagem é repetidamente movida para baixo e reposicionada acima do topo da tela para criar a ilusão de continuidade. Ela pode ser usada para animar o fundo de um jogo, por exemplo.
            </v-card-text>
          </v-expansion-panel-content>
        </v-expansion-panel>
      </v-expansion-panels>
    </v-row>
  </v-card>
  <v-card class="mt-5 ml-3 mr-3">
    <v-row justify="center">
      <v-expansion-panels accordion>
        <v-expansion-panel>
          <v-expansion-panel-header><v-toolbar-title>Button</v-toolbar-title></v-expansion-panel-header>
          <v-expansion-panel-content>
            <v-img src="../assets/button_class.png"></v-img>
            <v-card-title>
              A classe Button é usada para criar um botão interativo na interface gráfica de um jogo ou aplicação desenvolvida com Pygame. Vamos analisar o que cada parte dessa classe faz:
            </v-card-title>
            <v-card-subtitle>
                <v-card-subtitle>
                def __init__(self, color, x, y, text, callback): O construtor da classe Button recebe a cor do botão (color), as coordenadas X e Y (x e y), o texto do botão (text) e uma função de retorno (callback) como argumentos.
                  
                </v-card-subtitle>
                <v-card-subtitle>
               self.display = pygame.display.get_surface(): Retorna a superfície atual associada à janela principal do Pygame. Essa superfície é armazenada no atributo self.display e será usada posteriormente para desenhar o botão.

                </v-card-subtitle>
                <v-card-subtitle>
              self.color = color: Armazena a cor do botão no atributo self.color.

                </v-card-subtitle>
                <v-card-subtitle>

              self.rect = pygame.Rect(x, y, 250, 50): Cria um objeto pygame.Rect com as coordenadas e dimensões do botão. O retângulo representa a área do botão na tela.
                </v-card-subtitle>
                <v-card-subtitle>

              self.text_color = 'white': Armazena a cor do texto do botão no atributo self.text_color.
                </v-card-subtitle>
                <v-card-subtitle>
              self.text_position = [(x + self.rect.width / 2), (y + self.rect.height / 2)]: Calcula a posição central do botão com base nas coordenadas fornecidas e no tamanho do retângulo. Essa posição é armazenada no atributo self.text_position.

                </v-card-subtitle>
                <v-card-subtitle>
              self.text = text: Atribui o texto do botão ao atributo self.text.

                </v-card-subtitle>
                <v-card-subtitle>
              self.render = Text('assets/assets_pong/fonts/Retro_Gaming.ttf', 40, self.text, self.text_color, self.text_position): Cria uma instância da classe Text (provavelmente uma classe personalizada) para renderizar o texto do botão com uma fonte específica, tamanho, cor e posição.

                </v-card-subtitle>
                <v-card-subtitle>
              self.call_back = callback: Atribui a função de retorno (callback) ao atributo self.call_back.

                </v-card-subtitle>
                <v-card-subtitle>
              self.active = False: Inicializa o atributo self.active como falso. Esse atributo pode ser usado para controlar o estado do botão (ativo ou inativo).

                </v-card-subtitle>
                <v-card-subtitle>
              def events(self, event): O método events é chamado para lidar com eventos relacionados ao botão, como movimento do mouse e cliques.

                </v-card-subtitle>
                <v-card-subtitle>
              if event.type == pygame.MOUSEMOTION:: Verifica se ocorreu um evento de movimento do mouse.

                </v-card-subtitle>
                <v-card-subtitle>
              if self.rect.collidepoint(event.pos):: Verifica se a posição do evento de movimento do mouse está dentro da área do botão. Se sim, atualiza o texto do botão para exibir a cor vermelha.

                </v-card-subtitle>
                <v-card-subtitle>
              else:: Caso contrário, atualiza o texto do botão para exibir a cor amarela.

                </v-card-subtitle>
                <v-card-subtitle>
              if event.type == pygame.MOUSEBUTTONDOWN:: Verifica se ocorreu um evento de clique do mouse.

                </v-card-subtitle>
                <v-card-subtitle>
              if event.button == 1 and self.rect.collidepoint(event.pos):: Verifica se o botão esquerdo do mouse foi clicado e se a posição do clique está dentro da área do botão. Se sim, chama a função de retorno (callback) atribuída ao botão.

                </v-card-subtitle>
                <v-card-subtitle>
              def draw(self): O método draw é responsável por desenhar o botão na tela.

                </v-card-subtitle>
                <v-card-subtitle>
              pygame.draw.rect(self.display, self.color, self.rect): Desenha o retângulo do botão na superfície de exibição (self.display) usando a cor do botão (self.color) e as dimensões definidas pelo retângulo (self.rect).

                </v-card-subtitle>
                <v-card-subtitle>
              self.render.draw_center(): Chama um método draw_center na instância da classe Text (provavelmente personalizada) para renderizar o texto do botão centralizado dentro da área do botão.

                </v-card-subtitle>

            </v-card-subtitle>
            <v-card-title>
              Essa classe encapsula a lógica de um botão interativo, permitindo que ele seja desenhado na tela, responda a eventos de movimento do mouse e cliques do mouse, e execute uma função de retorno quando clicado. É útil para criar interfaces de usuário com botões interativos em jogos ou aplicativos feitos com Pygame.
              </v-card-title>
              </v-expansion-panel-content>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-row>
      </v-card>
    </v-container>
  </div>
</template>

<script>
  export default {}

</script>

<style lang="css">

.theme--dark.v-data-table tbody tr:nth-of-type(even) {
    background-color: rgba(85, 85, 85, 0.5);
}

</style>