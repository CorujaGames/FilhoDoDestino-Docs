# Tema 6: Nivelamento

## Épico 6.1: Progresso por experiência e evolução de atributos

### US35 - Ganhar experiência por exploração e combate

#### **História de usuário**  
Como jogador, quero ganhar XP ao derrotar inimigos e explorar áreas, para progredir no nivelamento do personagem.

#### **Critérios de aceitação**  
- O sistema deve conceder XP ao derrotar inimigos em combate.  
- Explorar regiões inexploradas do mapa também gera XP.  
- O acúmulo de XP deve ser visível ao jogador em tempo real.

#### **Regras de negócio**  
- O XP ganho varia conforme a dificuldade do inimigo e a raridade da área descoberta.  
- A quantidade de XP é registrada mesmo que o jogador não suba de nível imediatamente.

#### **Análise de risco**  
Valor: 5 – Urgência: 4 – Risco: 2 – Esforço: 3 – Dependência: 3 – Prioridade: 17

### US36 - Aumentar a probabilidade de habilidades mais fortes

#### **História de usuário**  
Como jogador, quero que o avanço de nível aumente a chance de aparecerem habilidades de grau mais alto, para evoluir minhas estratégias de forma coerente.

#### **Critérios de aceitação**  
- A cada novo nível, o sistema ajusta a probabilidade de habilidades avançadas surgirem nas escolhas.  
- A mudança na distribuição de probabilidade deve ser informada visualmente ao jogador.  
- Habilidades comuns continuam disponíveis, mas com menor frequência.

#### **Regras de negócio**  
- A chance de habilidades mais fortes aumenta de forma gradual e acumulativa por nível.  
- Jogadores com níveis baixos não podem receber habilidades de grau final.

#### **Análise de risco**  
Valor: 5 – Urgência: 3 – Risco: 3 – Esforço: 3 – Dependência: 3 – Prioridade: 16

### US37 - Distribuir pontos de atributo após retorno

#### **História de usuário**  
Como jogador, quero distribuir pontos de atributo fixos ao retornar, para melhorar velocidade, ataque e defesa dos personagens upados.

#### **Critérios de aceitação**  
- O jogador recebe pontos de atributo ao retornar de uma partida (mesmo após falha).  
- Os pontos podem ser alocados em atributos específicos: velocidade, ataque ou defesa.  
- A distribuição afeta o desempenho nas próximas tentativas.

#### **Regras de negócio**  
- Os pontos de atributo são permanentes até nova redistribuição autorizada.  
- A alocação só pode ser feita em momentos específicos (ex: ponto de Cáronte).

#### **Análise de risco**  
Valor: 5 – Urgência: 4 – Risco: 3 – Esforço: 3 – Dependência: 4 – Prioridade: 18
