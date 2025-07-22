# Tema 2: Habilidades

## Épico 2.1: Progressão de habilidades e árvore de escolhas

### US13 - Estruturar habilidades em árvore

#### **História de usuário**  
Como jogador, quero que o sistema de habilidades seja organizado em formato de árvore de escolhas, para desenvolver caminhos estratégicos diferentes.

#### **Critérios de aceitação**  
- As habilidades devem ser organizadas em uma estrutura hierárquica com ramificações.  
- Só é possível desbloquear habilidades com pré-requisitos atendidos.

#### **Regras de negócio**  
 - Habilidades de grau maior dependem do nivel do personagem.
 - Habilidades podem necessitar de habilidades anteriores.

#### **Análise de risco**  
Valor: 5 – Urgência: 4 – Risco: 3 – Esforço: 4 – Dependência: 4 – Prioridade: 17


### US14 - Apresentar três fios do destino

#### **História de usuário**  
Como jogador, quero visualizar três opções de habilidade a cada subida de nível, para escolher uma e construir minha progressão.

#### **Critérios de aceitação**  
- Ao subir de nível, o jogador recebe três habilidades aleatórias elegíveis.  
- Apenas uma habilidade pode ser selecionada.  
- As opções devem variar com base na árvore já construída.

#### **Regras de negócio**  
- As habilidades oferecidas devem ser compatíveis com o progresso atual do jogador.  
- Habilidades repetidas não devem ser ofertadas.

#### **Análise de risco**  
Valor: 4 – Urgência: 3 – Risco: 2 – Esforço: 3 – Dependência: 3 – Prioridade: 14

## Épico 2.2: Morte e permanência

### US15 - Retornar ao ponto de Cáronte para reviver

#### **História de usuário**  
Como jogador, quero que personagens abatidos possam ser revividos no último ponto de Cáronte.

#### **Critérios de aceitação**  
- Após serem abatidos, personagens retornam ao último ponto de Cáronte salvo.  
- O sistema exibe animação ou mensagem de retorno.  
- Progresso desde o último ponto é perdido.

#### **Regras de negócio**  
- Apenas personagens com salvamento ativo em Cáronte podem ser revividos.  
- Eventos entre o salvamento e a morte não são restaurados.

#### **Análise de risco**  
Valor: 4 – Urgência: 4 – Risco: 2 – Esforço: 3 – Dependência: 3 – Prioridade: 15


### US16 - Reiniciar do início em caso de morte

#### **História de usuário**  
Como jogador, quero que a morte total reinicie o jogo na primeira etapa do mapa atual, para que a progressão tenha riscos reais.

#### **Critérios de aceitação**  
- Ao todos os personagens morrerem, perdem o progresso atual e reinicia no início do mapa.  
- Itens e bônus temporários são resetados.  
- O sistema confirma o reinício ao jogador.

#### **Regras de negócio**  
- O progresso permanente (como habilidades fixas) não é perdido.  
- A reinicialização ocorre automaticamente após a morte total.

#### **Análise de risco**  
Valor: 4 – Urgência: 4 – Risco: 2 – Esforço: 2 – Dependência: 2 – Prioridade: 14


### US17 - Selecionar uma habilidade fixa após a morte

#### **História de usuário**  
Como jogador, quero escolher uma habilidade para manter permanentemente após morrer, para evoluir o personagem mesmo com reinícios.

#### **Critérios de aceitação**  
- Após a morte, o jogador escolhe uma entre as habilidades adquiridas para manter.  
- A habilidade fixa estará disponível nas próximas partidas.  
- A escolha é feita antes de reiniciar a jornada.

#### **Regras de negócio**  
- A habilidade fixa não pode ser trocada.  
- Habilidades de evento único não podem ser fixadas.

#### **Análise de risco**  
Valor: 5 – Urgência: 4 – Risco: 3 – Esforço: 3 – Dependência: 4 – Prioridade: 17

## Épico 2.3: Subida de nível

### US18 - Ganhar pontos de habilidade por nível

#### **História de usuário**  
Como jogador, quero ganhar novas habilidades a cada nível atingido, para expandir as capacidades do personagem durante a jornada.

#### **Critérios de aceitação**  
- Cada novo nível concede pontos para desbloquear habilidades.  
- O jogador é notificado do ganho de ponto.  
- A árvore de habilidades é atualizada dinamicamente.

#### **Regras de negócio**  
- Pontos não utilizados permanecem acumulados.  
- Níveis repetidos não concedem habilidades duplicadas.

#### **Análise de risco**  
Valor: 5 – Urgência: 5 – Risco: 2 – Esforço: 2 – Dependência: 3 – Prioridade: 18


### US19 - Permitir subir de nível

#### **História de usuário**  
Ao estar em um ponto de Cáronte, permite subir de nível.

#### **Critérios de aceitação**  
- O jogador pode acessar a tela de evolução ao interagir com Cáronte.  
- O sistema exibe as habilidades disponíveis e pontos acumulados.  
- A evolução é confirmada e aplicada imediatamente.

#### **Regras de negócio**  
- Subida de nível só ocorre em pontos de Cáronte.  
- A disponibilidade de habilidades depende da árvore atual.

#### **Análise de risco**  
Valor: 4 – Urgência: 4 – Risco: 2 – Esforço: 2 – Dependência: 3 – Prioridade: 15
