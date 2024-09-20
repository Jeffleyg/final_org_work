# Jogo de Conexão 4 em Assembly - RISC-V

Este é um projeto de um jogo clássico de **Conexão 4** implementado em Assembly para a arquitetura RISC-V, utilizando o simulador **RARS**. O objetivo do jogo é alinhar quatro peças (verticais, horizontais ou diagonais) no tabuleiro antes do adversário.

## Funcionalidades

- **Dois modos de tabuleiro**:
  - Tabuleiro 7x6 (7 colunas e 6 linhas)
  - Tabuleiro 9x6 (9 colunas e 6 linhas)
  
- **Modo de jogo para 2 jogadores**:
  - Jogador 1 é representado por "X" (valor 1 no tabuleiro)
  - Jogador 2 é representado por "O" (valor 2 no tabuleiro)
  
- **Alternância de turnos**: Os jogadores alternam suas jogadas até que um deles vença ou o jogo termine em empate.

## Como jogar

1. Ao iniciar o programa, o **menu principal** será exibido com as opções:
   - **Configuração**: Permite ajustar o número de jogadores, o tamanho do tabuleiro, a dificuldade, e outras configurações.
   - **Jogar**: Começa o jogo diretamente com o tabuleiro configurado.
   - **Sair**: Encerra o programa.

2. Escolha o tamanho do tabuleiro no menu de configuração:
   - **7x6** para um tabuleiro menor.
   - **9x6** para um tabuleiro maior.

3. Após iniciar o jogo, o tabuleiro será exibido e os jogadores podem começar a jogar alternadamente.

4. **Jogador 1** começa sempre primeiro e deve escolher uma coluna para jogar. A jogada será marcada no ponto mais baixo disponível dessa coluna.

5. O **Jogador 2** fará o mesmo, até que um jogador alinhe 4 peças ou o tabuleiro esteja cheio (empate).

## Requisitos

- Simulador **RARS** (RISC-V Assembler and Runtime Simulator).
- Arquitetura **RISC-V**.

## Como rodar

1. Abra o **RARS**.
2. Carregue o arquivo `.asm` do projeto.
3. Execute o programa.
4. Siga as instruções no terminal para configurar e jogar.

## Estrutura do projeto

- **Menu principal**: Exibe opções de configuração e início do jogo.
- **Configuração**: Permite escolher o tamanho do tabuleiro e ajustar outras preferências.
- **Jogo**: Alterna entre os turnos dos jogadores, verifica a validade das jogadas e atualiza o tabuleiro após cada jogada.
- **Verificação de vitória**: Inclui uma função para verificar se um jogador conseguiu alinhar quatro peças consecutivas.

---
