# Chess System Java
Este projeto é um sistema de jogo de xadrez completo, desenvolvido em Java, que utiliza conceitos avançados de Programação Orientada a Objetos (POO). O jogo é executado inteiramente no terminal, com uma interface de linha de comando colorida.

## Sobre o Projeto
O objetivo deste projeto foi aplicar conhecimentos de herança, polimorfismo, encapsulamento e tratamento de exceções numa aplicação prática e lógica. O sistema gere todas as regras do xadrez, incluindo movimentos especiais e deteção de estados de jogo.

## Funcionalidades Implementadas:
Movimentos Básicos: Suporte para todas as peças (Rei, Rainha, Bispo, Cavaleiro, Torre e Peão) com as suas respetivas regras de movimento.

## Movimentos Especiais:

Roque (Castling): Tanto para o lado do rei quanto para o lado da rainha.

En Passant: Captura especial de peões.

Promoção: Quando um peão atinge a extremidade oposta do tabuleiro.

## Lógica de Jogo:

Sistema de turnos entre jogadores (Brancas e Pretas).

Deteção de Check e Checkmate.

Interface de utilizador que destaca as jogadas possíveis para a peça selecionada.

Contabilização de peças capturadas.

## Arquitetura do Sistema:
O projeto está dividido em camadas para melhor organização e manutenção:

Camada de Tabuleiro (Boardgame): Contém a lógica genérica para um tabuleiro e peças, incluindo deteção de posições e tratamento de erros através da BoardException.

Camada de Xadrez (Chess): Especializa a camada de tabuleiro para as regras específicas do xadrez, lidando com cores de peças e posições no formato a1 a h8.

Camada de Aplicação: Responsável pela interação direta com o utilizador, entrada de dados via teclado e renderização do tabuleiro no terminal.

## Tecnologias Utilizadas
Linguagem: Java 22.

IDE Utilizada: IntelliJ IDEA.

Controle de Versão: Git.

## Como Executar?
Para correr o projeto localmente, siga estes passos:

### 1. Clonar o repositório:
```git clone https://github.com/seu-utilizador/chess-system-java.git```

### 2. Compilar o projeto:
Navegue até à pasta src e compile os ficheiros .java.

### 3. Executar a aplicação:
Execute a classe Program localizada no pacote application:

```java application.Program```

## Como Jogar:
1. O tabuleiro será exibido no terminal.
2. Insira a posição da peça que deseja mover (ex: e2).
3. O sistema destacará em azul os movimentos possíveis.
4. Insira a posição de destino (ex: e4).
5. Continue os turnos até que ocorra um Checkmate.

>Nota: O projeto utiliza códigos ANSI para cores no terminal. Certifique-se de que o seu terminal suporta estas sequências para uma melhor experiência visual.