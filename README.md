# Gwent-Physical-and-Digital-Game

Resumo

"Gwent Board" é o projeto de um tabuleiro para 2 jogadores que mistura interações físicas e digitais.
É baseado inteiramente no jogo Gwent, na sua versão presente em The Witcher 3 - Wild Hunt, com ligeiras modificações.

Direitos

Gwent e The Witcher são marcas registradas, bem como suas artes, regras, músicas e quaisquer outras criações. 
O projeto não pode ser vendido e não possui fins lucrativos. O projeto "Gwent Board" é destinado ao aprendizado e diversão pessoal.

Lista de peças

Raspberry pi model 3B
Leitor NFC RC522
Cartões NFC
Modulo Amplificador de áudio I2S max98357a
Auto-falante 3w 4ohms
Led Ws2812b
Swithes NO com LED
Ecrã HDMI 7"
Fonte alimentação 5V 2.5A
Cabos HDMI e USB
Componentes eletrónicos (resistores, capacitores, fios, jumpers)

Programação

Python, com os pacotes principais:
Pygame, RPi, rpi_ws281x, mfrc522.

Construção

O tabuleiro foi desenhado, impresso em 3D e gravado a laser.
### imagens ###

A interface apresentada no ecrã foi desenhada no Inkscape.
### imagens ###



Lógica de funcionamento

A programação é dividida em módulos python. 
O módulo main.py é responsável pelo loop principal do jogo, enquanto os demais executam ações adicionais ou controlam dispositivos eletrónicos.
O arquivo json é uma biblioteca que possui todos os dados das cartas. 
### diagrama ###
### imagens ###

As regras do jogo são similares ao jogo original, com a exceção de algumas cartas, que estão ausentes.

Exemplo da carta "herói", que não é afetada pelas cartas especiais.
- Simulação de cartas no tabuleiro.
### imagens ###
- Aplicacao da regra, idêntica ao jogo original.
### imagens ###

O jogo possui lógicas de proteção para evitar erros e jogadas indevidas. 
Por exemplo: Não é possível repetir cartas; a leitura duplicada é protegida; jogar cartas não permitidas; realizar ações não permitidas, etc...





