# Tema 4: Inventário

## Épico 4.1: Capacidade e gerenciamento de espaço

### US27 - Definir capacidade inicial do inventário

#### **História de usuário**  
Como jogador, quero que o inventário possua 9 espaços totais, para acomodar uma quantidade limitada de itens.

#### **Critérios de aceitação**  
- O sistema deve limitar o inventário padrão a 9 espaços.  
- O jogador não pode adicionar novos itens caso o inventário esteja cheio.  
- Um aviso deve ser exibido quando a capacidade máxima for atingida.

#### **Regras de negócio**  
- A capacidade base é fixa e poderá ser expandida apenas por habilidades ou itens específicos.  
- Espaços ocupados não podem ser reutilizados até o descarte ou uso do item.

#### **Análise de risco**  
Valor: 4 – Urgência: 4 – Risco: 2 – Esforço: 2 – Dependência: 3 – Prioridade: 15

### US28 - Armazenar itens básicos

#### **História de usuário**  
Como jogador, quero guardar itens como poção de cura, poção de velocidade, espadinha e gema, para utilizar durante a exploração e combate.

#### **Critérios de aceitação**  
- O sistema deve permitir armazenar diferentes tipos de itens de uso rápido.  
- Os itens devem ser consumíveis ou equipáveis conforme a situação.  
- O jogador deve poder visualizar os itens disponíveis no inventário.

#### **Regras de negócio**  
- Itens têm tipos e categorias com efeitos distintos.  
- Poções são consumidas ao uso; armas e gemas são persistentes até troca ou descarte.

#### **Análise de risco**  
Valor: 5 – Urgência: 4 – Risco: 2 – Esforço: 2 – Dependência: 3 – Prioridade: 16

## Épico 4.2: Organização visual e por personagem

### US29 - Organizar itens no estilo Resident Evil

#### **História de usuário**  
Como jogador, quero organizar os itens visualmente em um grid com encaixe e rotação, para otimizar o uso do espaço disponível.

#### **Critérios de aceitação**  
- O sistema deve apresentar o inventário em um grid visual.  
- Itens possuem tamanhos diferentes e podem ser rotacionados.  
- O jogador pode mover e reposicionar itens livremente dentro do espaço.

#### **Regras de negócio**  
- A rotação consome um comando ou clique extra.  
- A colocação do item só é válida se houver espaço contínuo disponível.

#### **Análise de risco**  
Valor: 5 – Urgência: 5 – Risco: 3 – Esforço: 4 – Dependência: 4 – Prioridade: 18

### US30 - Definir inventário por personagem

#### **História de usuário**  
Como jogador, quero que cada personagem tenha seu próprio inventário com até 9 espaços, para personalizar os recursos de cada um.

#### **Critérios de aceitação**  
- Cada personagem possui um inventário independente.  
- O sistema permite alternar entre os inventários dos personagens.  
- Recursos não são compartilhados automaticamente entre personagens.

#### **Regras de negócio**  
- A transferência de itens entre personagens exige comando explícito.  
- A limitação de espaços é mantida para todos os personagens igualmente.

#### **Análise de risco**  
Valor: 5 – Urgência: 4 – Risco: 3 – Esforço: 3 – Dependência: 3 – Prioridade: 17
