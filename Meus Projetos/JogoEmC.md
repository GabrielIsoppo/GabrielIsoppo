# ⚔️ Knight's Exploration

Este é um jogo de plataforma 2D desenvolvido em linguagem C, onde o jogador controla uma cavaleira em um cenário com obstáculos e desafios. O projeto foi criado como parte de um trabalho prático da faculdade para aplicar conceitos de lógica de programação, loops e renderização gráfica usando a biblioteca Allegro5.


## 🚀 Principais Funcionalidades

* **Movimentação e física básica:** Controle de andar, pular, agachar e colidir com as plataformas do cenário de forma fluida.
* **Pulo adaptável:** A altura do pulo é baseada no tempo em que o botão de pular é pressionado.
* **Estrutura da fase:** O jogo avança conforme o jogador progride pelo mapa.
* **Sistema de HP e invulnerabilidade:** O jogador tem 2 HP (hit points) e, ao receber dano, entra em estado de invulnerabilidade por 1,5 segundo.
* **Seleção de dificuldade:** O nível pode ser alterado no menu principal e modifica a velocidade de movimento dos inimigos.


## 🛠️ Tecnologias e Ferramentas Utilizadas

* **Linguagem C:** Para construir toda a lógica do jogo, gerenciamento de estados e movimentação dos inimigos.
* **Allegro5:** Biblioteca utilizada para gerenciar a criação da tela e os eventos de forma intuitiva, permitindo o foco no desenvolvimento das mecânicas.
* **Make (Makefile):** Disponibilizado pelos professores para facilitar a compilação e os testes.
* **Valgrind:** Para testes de vazamentos de memória (memory leaks).


## 🧠 Desafios Técnicos e Aprendizados

### Física do jogo
* **O problema:** Foi a minha primeira vez lidando com a implementação de física para um jogo.
* **A solução:** Meu objetivo era que a física fosse parecida com a do primeiro jogo do Mario (*Super Mario Bros.*), visto que ela é bem fluida e confortável de jogar. Para alcançar isso, passei bastante tempo testando e ajustando os valores até encontrar o comportamento ideal.

### Colisão com plataformas
* **O problema:** Entender as condições lógicas e como tratar as colisões no cenário.
* **A solução:** Realizei testes incessantes para buscar qualquer brecha ou falha no mapa. Como eu naturalmente gosto de procurar bugs em jogos, apliquei essa mentalidade no meu próprio projeto. Essa rotina de testes me ajudou a entender como estruturar as checagens de colisão e quais parâmetros corretos eu deveria utilizar.

### Gerenciamento de estados e animações da personagem
* **O problema:** Controlar as transições de animações e as regras de cada estado da cavaleira.
* **A solução:** A personagem possui vários estados (andando, ociosa, pulando, agachando, escalando). Para tratar quando cada uma acontece, utilizei variáveis de controle dentro da estrutura (`struct`) da jogadora para disparar a animação correta. Além disso criei uma lógica que deixa de renderizar a personagem a cada 4 frames, criando o efeito de piscar quando está no estado de invunerabilidade.

💻 Desenvolvido por **Gabriel de Souza Isoppo** — Entre em contato no [LinkedIn](https://www.linkedin.com/in/gabriel-de-souza-isoppo-a7630739b/).

##### 🤖 *Nota: Esta documentação utilizou inteligência artificial estritamente para a estruturação do template (Markdown) e revisão ortográfica das descrições autorais.*