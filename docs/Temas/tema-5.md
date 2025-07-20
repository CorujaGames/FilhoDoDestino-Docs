# Tema 5: Comunicação

## Épico 5.1: Interações com personagens não jogáveis (NPCs)

### US31 - Implementar sistema de diálogo com NPCs

#### **História de usuário**  
Como jogador, quero conversar com NPCs espalhados pelo mapa, para obter informações sobre o mundo, a história e os personagens.

#### **Critérios de aceitação**  
- O jogador pode iniciar diálogos com NPCs interativos.  
- O sistema apresenta texto correspondente à fala do personagem.  
- A interação pode ocorrer em diferentes partes do mapa.

#### **Regras de negócio**  
- NPCs só podem iniciar diálogo quando em estado acessível (fora de combate).  
- Algumas falas podem se repetir até que novos eventos sejam liberados.

#### **Análise de risco**  
Valor: 5 – Urgência: 4 – Risco: 3 – Esforço: 3 – Dependência: 3 – Prioridade: 17

### US32 - Descobrir tópicos de diálogo

#### **História de usuário**  
Como jogador, quero desbloquear novos tópicos de conversa explorando o mapa, para expandir o conteúdo disponível nos diálogos.

#### **Critérios de aceitação**  
- Ao visitar locais ou coletar itens, o jogador desbloqueia novos assuntos.  
- O sistema indica visualmente quais tópicos são inéditos.  
- NPCs reagem aos tópicos conforme contexto da jornada.

#### **Regras de negócio**  
- Tópicos só são disponibilizados se o pré-requisito de exploração for cumprido.  
- Os tópicos desbloqueados permanecem no histórico do jogador.

#### **Análise de risco**  
Valor: 4 – Urgência: 4 – Risco: 2 – Esforço: 3 – Dependência: 3 – Prioridade: 15

### US33 - Escolher tópicos durante a conversa

#### **História de usuário**  
Como jogador, quero selecionar tópicos específicos ao interagir com um NPC, para direcionar a conversa conforme meu interesse.

#### **Critérios de aceitação**  
- O sistema apresenta uma lista de tópicos ao iniciar o diálogo.  
- O jogador pode escolher qualquer tópico desbloqueado.  
- Cada seleção gera uma resposta correspondente do NPC.

#### **Regras de negócio**  
- O número de tópicos disponíveis varia conforme o progresso.  
- Alguns tópicos podem desaparecer após uso, outros se manterão acessíveis.

#### **Análise de risco**  
Valor: 5 – Urgência: 4 – Risco: 2 – Esforço: 3 – Dependência: 3 – Prioridade: 16

### US34 - Exibir respostas dubladas dos NPCs

#### **História de usuário**  
Como jogador, quero que as falas dos NPCs sejam dubladas ao escolher um tópico, para tornar a experiência mais imersiva.

#### **Critérios de aceitação**  
- Ao selecionar um tópico, a fala correspondente do NPC é reproduzida com voz.  
- O texto e o áudio devem estar sincronizados.  
- O jogador pode ativar ou desativar a dublagem nas configurações.

#### **Regras de negócio**  
- As falas devem corresponder ao idioma do jogo.  
- NPCs silenciosos ou criaturas sem linguagem compreensível não têm dublagem.

#### **Análise de risco**  
Valor: 5 – Urgência: 3 – Risco: 3 – Esforço: 4 – Dependência: 4 – Prioridade: 16
