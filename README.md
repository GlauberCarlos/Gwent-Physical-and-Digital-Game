# 🧩 Projeto: Gwent-Physical-and-Digital-Game
"Gwent Board" é o projeto de um tabuleiro para 2 jogadores que mistura interações físicas e digitais.
É baseado inteiramente no jogo Gwent, na sua versão presente em The Witcher 3 - Wild Hunt, com ligeiras modificações.

---

📌 Direitos:
- Gwent e The Witcher são marcas registradas, bem como suas artes, regras, músicas e quaisquer outras criações. 
O projeto não pode ser vendido e não possui fins lucrativos. O projeto "Gwent Board" é destinado ao aprendizado e diversão pessoal.

---

## 🛠️ Lista de peças

- Raspberry pi model 3B
- Leitor NFC RC522
- Cartões NFC
- Modulo Amplificador de áudio I2S max98357a
- Auto-falante 3w 4ohms
- Led Ws2812b
- Swithes NO com LED
- Ecrã HDMI 7"
- Fonte alimentação 5V 2.5A
- Cabos HDMI e USB
- Componentes eletrónicos (resistores, capacitores, fios, jumpers)

---

## Programação

Python, os pacotes principais são:
- Pygame, RPi, rpi_ws281x, mfrc522.
---
## Processo de criação/construção

- Criei a lógica de programação e algoritmos, obtive muito auxílio do ChatGPT com a linguagem Python, bem como a instalação das libs e interação com os pacotes e dispositivos.
- Os inputs de eletrônica e ligações ao Raspberry pi foram dados pelo ChatGPT.
- O design 2D das cartas, impressão e adesivos foram feitos por mim.
- O design apresentado no ecrã foi feito por mim.
- O projeto do tabuleiro e a impressão em 3D foram feitas por mim.
- A gravação dos desenhos no tabuleiro foram feitas por mim.
- As músicas em background são originais do jogo Gwent, versão "The Witcher 3 - Wild Hunt".
- Alguns efeitos sonoros são originais do jogo Gwent, outros são sons genéricos editados.

### imagens ###

---

## ⚙️ Lógica de funcionamento

- A programação é dividida em módulos python. 
- O módulo main.py é responsável pelo loop principal do jogo, enquanto os demais módulos executam ações adicionais ou controlam dispositivos eletrónicos.
- O arquivo json é uma biblioteca que possui todos os dados das cartas. 
### diagrama ###
### imagens ###
---
## 🎯 Jogo em si

As regras do jogo são similares ao do jogo Gwent original, com a exceção de algumas cartas, que estão ausentes.
Fluxo explicado abaixo:

- Jogo por turnos. Cada carta jogada passa pelo sensor, que contabiliza a pontuação, realiza uma função específica ou aguarda alguma decisão do jogador.
- A carta jogada deverá ir para o local determinado.
- A rodada acaba quando ambos os jogadores "passam a vez". O jogador sem cartas passa a vez automaticamente.
- Quem tiver maior pontuação vence a rodada.
- As cartas da rodada recém-terminada vão para o lixo.
- Inicia-se uma nova rodada com as cartas que sobraram nas mãos.
- Quem vencer mais rodadas (de 3), ganha o jogo.
  
---
Exemplo da carta "herói", que não é afetada pelas cartas especiais.
- Simulação de cartas no tabuleiro.
### imagens ###
- Aplicacao da regra, idêntica ao jogo original.
### imagens ###

--- 

O jogo possui lógicas de proteção para evitar erros e jogadas indevidas. 
Por exemplo: Não é possível repetir cartas; a leitura duplicada é protegida; não é possíveljogar cartas não permitidas no momento, etc...






