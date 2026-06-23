# ANACONDA - Jogo estilo Snake

Este repositório contém o desenvolvimento do jogo **ANACONDA**, um protótipo baseado no clássico *Snake*, desenvolvido em Python utilizando a biblioteca **Pygame**[cite: 2]. O projeto atende aos requisitos do ponto de controle PC03 da disciplina.

## 👥 Integrantes do Grupo
* **Guilherme Miranda Nascimento**[cite: 2]

---

## 🎮 Sobre o Jogo e Objetivo
O objetivo principal é controlar uma cobra que se move por uma grade para coletar os alimentos que surgem aleatoriamente[cite: 2]. Cada alimento consumido aumenta a pontuação do jogador em 10 pontos e faz a cobra crescer de tamanho[cite: 2]. 

O jogo possui um sistema de persistência que salva o maior recorde localmente em um arquivo de texto.

### Regras Principais:
1. **Controles:** O movimento é realizado inteiramente através das setas do teclado[cite: 2].
2. **Condição de Derrota:** O jogo possui **1 vida**[cite: 2]. A partida se encerra imediatamente (Game Over) caso a cobra colida com as bordas da tela ou com o seu próprio corpo[cite: 2].
3. **Condição de Vitória:** Ocorre se o jogador conseguir preencher todo o tabuleiro sem sofrer nenhuma colisão[cite: 2].

---

## 🕹️ Controles
* ⬆️ **Seta para Cima:** Move para cima[cite: 2]
* ⬇️ **Seta para Baixo:** Move para baixo[cite: 2]
* ⬅️ **Seta para Esquerda:** Move para esquerda[cite: 2]
* ➡️ **Seta para Direita:** Move para direita[cite: 2]
* ⎵ **Espaço (Na tela de Game Over):** Reinicia a partida
* ⎋ **ESC (Na tela de Game Over):** Fecha o jogo

---

## 📁 Organização do Código
O projeto foi modularizado seguindo estritamente a arquitetura planejada na proposta inicial[cite: 2]:

* `main.py`: Ponto de entrada que inicializa o Pygame e dispara o loop[cite: 2].
* `ranking.txt`: Arquivo gerado automaticamente que armazena a maior pontuação alcançada de forma persistente.
* `src/config.py`: Centraliza as constantes do jogo como cores, dimensões e taxa de atualização (FPS)[cite: 2].
* `src/cobra.py`: Contém a classe que gerencia o corpo, crescimento e mudança de direção da cobra[cite: 2].
* `src/comida.py`: Cuida do posicionamento randômico e renderização dos alimentos[cite: 2].
* `src/telas.py`: Controla o menu gráfico de fim de jogo e a leitura/escrita do High Score[cite: 2].
* `src/jogo.py`: Concentra o motor principal do jogo, computando colisões e alternando os estados do loop[cite: 2].

---

## 🚀 Como Executar o Jogo

### Pré-requisitos
Certifique-se de ter o Python 3 e o gerenciador de pacotes `pip` instalados no seu computador.

1. Abra o terminal na pasta raiz do projeto e instale a dependência do Pygame:
```bash
   pip install pygame
