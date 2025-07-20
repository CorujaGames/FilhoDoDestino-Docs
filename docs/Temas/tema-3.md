# Tema 3: Exploração

## Épico 3.1: Integração entre exploração e combate

### US20 - Integrar exploração e combate

#### **História de usuário**  
Como jogador, quero que o combate por turnos se inicie automaticamente ao entrar em contato com criaturas, para manter a fluidez entre exploração e batalha.

#### **Critérios de aceitação**  
- Ao tocar a área de uma criatura hostil durante a exploração, inicia-se automaticamente um combate por turnos.  
- A transição entre exploração e combate deve ser fluida e visualmente clara.  
- O jogador deve manter a formação dos personagens no início do combate.

#### **Regras de negócio**  
- A transição deve ocorrer sem necessidade de carregamento manual.  
- Inimigos só iniciam combate se estiverem em estado hostil.

#### **Análise de risco**  
Valor: 5 – Urgência: 4 – Risco: 3 – Esforço: 4 – Dependência: 4 – Prioridade: 17

## Épico 3.2: Progresso espacial e tomada de decisão

### US21 - Definir o avanço por portas

#### **História de usuário**  
Como jogador, quero que o acesso aos próximos mapas dependa das portas encontradas, para que o progresso seja construído com base nas minhas escolhas.

#### **Critérios de aceitação**  
- Ao final de cada mapa, o jogador encontra múltiplas portas com destinos diferentes.  
- O jogador pode escolher apenas uma porta por avanço.  
- As portas devem ser visivelmente distintas entre si.

#### **Regras de negócio**  
- Portas acessadas são registradas no histórico do jogador.  
- Portas não acessadas são descartadas permanentemente.

#### **Análise de risco**  
Valor: 4 – Urgência: 4 – Risco: 2 – Esforço: 3 – Dependência: 3 – Prioridade: 15

### US22 - Acessar portas de exploração

#### **História de usuário**  
Como jogador, quero encontrar diferentes tipos de portas durante a exploração, para acessar novas áreas com recompensas, como ouro, monstros, itens, pontos de evolução (portas de Cáronte), áreas de diálogo e recrutamento (portas de acampamento), itens raros (portas de tesouro), combates desafiadores contra chefes (portas de boss) e áreas para acessar mapas e eventos principais (portas de lore).

#### **Critérios de aceitação**  
- Cada tipo de porta possui uma aparência única.  
- O jogador pode identificar o tipo de área associada antes de entrar.  
- Portas devem estar distribuídas de forma equilibrada nos mapas.

#### **Regras de negócio**  
- Portas são geradas de forma semirrandômica, respeitando os limites do mapa.  
- Áreas exclusivas só aparecem uma vez por partida.

#### **Análise de risco**  
Valor: 5 – Urgência: 5 – Risco: 3 – Esforço: 4 – Dependência: 5 – Prioridade: 19

### US23 - Progredir entre dois mundos

#### **História de usuário**  
Como jogador, quero explorar tanto o mundo comum quanto o submundo, para vivenciar diferentes desafios e descobertas ao longo da jornada.

#### **Critérios de aceitação**  
- O jogador pode alternar entre os dois mundos em locais específicos.  
- Cada mundo possui estética, inimigos e itens próprios.  
- A mudança de mundo impacta rotas, diálogos e eventos disponíveis.

#### **Regras de negócio**  
- Pontos de transição entre mundos são fixos e limitados.  
- Itens obtidos em um mundo podem ser necessários no outro.

#### **Análise de risco**  
Valor: 5 – Urgência: 4 – Risco: 3 – Esforço: 4 – Dependência: 4 – Prioridade: 17

## Épico 3.3: Retorno e exploração aprofundada

### US24 - Desbloquear áreas com itens adquiridos

#### **História de usuário**  
Como jogador, quero acessar áreas anteriormente bloqueadas utilizando itens coletados, para incentivar o retorno a locais já visitados.

#### **Critérios de aceitação**  
- Áreas inacessíveis inicialmente podem ser abertas com chaves, runas ou habilidades.  
- O sistema deve indicar visualmente quando o item necessário está disponível.  
- O retorno deve ser possível a partir de pontos de conexão no mapa.

#### **Regras de negócio**  
- O item de desbloqueio é consumido ou marcado como usado.  
- O mapa do jogador é atualizado ao desbloquear a nova área.

#### **Análise de risco**  
Valor: 4 – Urgência: 4 – Risco: 2 – Esforço: 3 – Dependência: 3 – Prioridade: 15

### US25 - Resolver puzzles ambientais

#### **História de usuário**  
Como jogador, quero resolver puzzles durante a exploração, para desbloquear recompensas, caminhos e interações com o ambiente.

#### **Critérios de aceitação**  
- O sistema apresenta desafios lógicos ou físicos integrados ao cenário.  
- A resolução deve abrir passagens, entregar itens ou liberar segredos.  
- Puzzles devem ter dificuldade progressiva.

#### **Regras de negócio**  
- Um puzzle resolvido não pode ser repetido.  
- Algumas áreas só podem ser acessadas após resolver todos os puzzles associados.

#### **Análise de risco**  
Valor: 4 – Urgência: 3 – Risco: 3 – Esforço: 4 – Dependência: 4 – Prioridade: 14

## Épico 3.4: Interações sociais durante a exploração

### US26 - Interagir com personagens no mapa

#### **História de usuário**  
Como jogador, quero interagir com NPCs e aliados durante a exploração, para descobrir histórias, obter recompensas e liberar novos personagens.

#### **Critérios de aceitação**  
- O jogador pode iniciar diálogos com NPCs e personagens encontrados.  
- Algumas interações desbloqueiam aliados jogáveis ou missões secundárias.  
- O sistema deve apresentar opções de resposta que influenciam o resultado.

#### **Regras de negócio**  
- Cada NPC possui um conjunto fixo de eventos ou diálogos.  
- Interações podem ser únicas ou condicionadas ao progresso.

#### **Análise de risco**  
Valor: 5 – Urgência: 4 – Risco: 2 – Esforço: 3 – Dependência: 3 – Prioridade: 16
