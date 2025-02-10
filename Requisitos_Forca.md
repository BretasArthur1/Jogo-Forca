# Documento de Requisitos do Jogo de Forca Online

## 1. Descrição Geral
O Jogo de Forca Online é uma aplicação web onde usuários podem:
- Criar salas de jogo individuais ou em grupo (multiplayer).
- Convidar outros usuários a participarem da partida.
- Adivinhar palavras dentro de um número limitado de tentativas, de acordo com as regras clássicas do jogo de forca.

## 2. Requisitos Funcionais

### 2.1. Cadastro e Autenticação
1. **RF001** - O sistema deve permitir que o usuário crie uma conta informando e-mail, nome de usuário e senha.
2. **RF002** - O sistema deve validar as credenciais do usuário (e-mail/usuário e senha) para permitir acesso ao jogo.
3. **RF003** - O sistema deve permitir recuperação de senha via e-mail cadastrado.

### 2.2. Partidas
4. **RF004** - O sistema deve permitir a criação de salas (partidas) tanto públicas quanto privadas.
5. **RF005** - O sistema deve permitir que os usuários entrem em salas públicas ou privadas (com código de acesso).
6. **RF006** - O sistema deve sortear automaticamente uma palavra para cada rodada.
7. **RF007** - O sistema deve permitir que os jogadores façam tentativas de letra durante a rodada.
8. **RF008** - O sistema deve exibir o número de tentativas restantes e o progresso de acertos da palavra.
9. **RF009** - O sistema deve registrar pontuação ou vitórias para cada jogador, caso seja um modo de competição.
10. **RF010** - O sistema deve permitir a criação de partidas em modo “single player” (jogador único), caso o usuário deseje jogar sozinho.

### 2.3. Multiplayer
11. **RF011** - O sistema deve possibilitar partidas multiplayer (mais de um jogador ao mesmo tempo).
12. **RF012** - O sistema deve mostrar o status de cada jogador (quem ainda pode jogar, quantas letras errou, etc.).
13. **RF013** - O sistema deve informar quando um jogador acertou a palavra ou quando todas as tentativas acabaram.

## 3. Requisitos Não Funcionais

1. **RNF001** - O sistema deve estar disponível em 24 horas por dia, 7 dias por semana, com downtime inferior a 1%.
2. **RNF002** - O carregamento inicial da tela de jogo deve ocorrer em menos de 3 segundos (em conexões banda larga).
3. **RNF003** - A aplicação deve ser responsiva e compatível com os principais navegadores e dispositivos móveis.
4. **RNF004** - O sistema deve armazenar dados de usuário e de partidas em um banco de dados seguro, garantindo confidencialidade.
5. **RNF005** - A aplicação deve ter logs de acesso e erros para auditoria e resolução de problemas.

## 4. Tecnologias e Observações
- Sugere-se o uso de uma stack web (por exemplo, Node.js + React ou outra tecnologia de preferência).
- Para banco de dados, sugere-se MySQL, PostgreSQL ou MongoDB, conforme a demanda.
- As partidas podem ser gerenciadas em tempo real utilizando tecnologias como WebSocket ou Socket.io.

---


