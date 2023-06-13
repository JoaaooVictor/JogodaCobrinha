# Jogo da Cobrinha em JavaScript

Este é um simples jogo da cobrinha implementado em JavaScript, onde o jogador controla uma cobra que precisa coletar objetos no tabuleiro. O jogo é executado em um elemento canvas e utiliza o contexto 2D para desenhar os elementos na tela.

## Funcionalidades

O jogo possui as seguintes funcionalidades:

- Iniciar o jogo clicando no botão "Iniciar".
- Controlar a direção da cobra usando as setas do teclado (cima, baixo, esquerda, direita).
- A cobra pode se mover nas quatro direções: cima, baixo, esquerda e direita.
- O objetivo do jogo é coletar os objetos vermelhos que aparecem aleatoriamente no tabuleiro.
- A cada objeto coletado, a pontuação aumenta em 1.
- Se a cobra colidir com as bordas do tabuleiro ou com seu próprio corpo, o jogo termina.
- Quando o jogo termina, uma mensagem de "Game Over" é exibida na tela.
- O jogo pode ser reiniciado clicando novamente no botão "Iniciar".

## Funções

O programa é dividido em várias funções para melhor organização e estruturação do código:

- `update()`: É a função principal do jogo. Ela é responsável por atualizar a posição da cobra, verificar colisões, gerar novos objetos, atualizar a tela e chamar recursivamente a si mesma para manter o jogo em execução.
- `handleKeyPress(event)`: É chamada quando uma tecla é pressionada. Ela verifica a tecla pressionada e atualiza a direção da cobra de acordo com a tecla pressionada pelo jogador.
- `gameOver()`: É chamada quando o jogo termina. Ela limpa a tela, exibe a mensagem "Game Over" e reinicia a pontuação.
- `document.addEventListener("DOMContentLoaded", () => { ... })`: É a função de inicialização do jogo. Ela é executada quando o documento HTML é carregado e define os eventos de clique do botão "Iniciar", de pressionar as teclas do teclado e inicia a execução da função `update()`.

## Executando o Jogo

Para executar o jogo, basta inserir o código JavaScript em um arquivo HTML e abri-lo em um navegador. Certifique-se de ter um elemento `<canvas>` com o id "gameCanvas" para renderizar o jogo e um botão com o id "inicia" para iniciar o jogo. O jogador pode controlar a cobra usando as setas do teclado e o objetivo é coletar os objetos vermelhos para aumentar a pontuação.

Divirta-se jogando o jogo da cobrinha!