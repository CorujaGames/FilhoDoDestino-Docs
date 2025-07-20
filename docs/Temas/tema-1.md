# Tema 1: Combate

## Épico 1.1: Execução de turnos e ações em combate

### US01 - Calcular a ordem dos turnos

**História de usuário**  
Como jogador, quero que a ordem dos turnos seja definida pela velocidade dos personagens, para garantir estratégias baseadas em agilidade.

**Critérios de aceitação**  
- O sistema deve calcular a ordem de turnos com base no atributo de velocidade de cada personagem.  
- A ordem deve ser exibida no início de cada rodada de combate.  
- Mudanças de velocidade por efeitos temporários devem alterar a ordem nas rodadas seguintes.

**Regras de negócio**  
- A ordem de turno é recalculada a cada nova rodada.  
- Em caso de empate de velocidade, o sistema deve aplicar um critério de desempate predefinido (ex: ID ou sorte).

**Análise de risco**  
Valor: 5 – Urgência: 4 – Risco: 2 – Esforço: 2 – Dependência: 3 – Prioridade: 16

**Protótipo relacionado a US**  
[Placeholder: imagem da interface de ordem de turno]

### US02 - Executar ações no turno

**História de usuário**  
Como jogador, quero escolher entre atacar, usar item, passar a vez ou fugir, para tomar decisões táticas durante o combate.

**Critérios de aceitação**  
- Durante seu turno, o jogador pode selecionar uma entre as opções disponíveis.  
- As ações devem ser executadas imediatamente ou programadas conforme regras de delay.  
- A opção de fugir só estará disponível se o combate permitir.

**Regras de negócio**  
- Fugir pode ser desabilitado contra chefes.  
- Usar item consome o item do inventário.  
- Passar turno não consome recursos, mas finaliza a vez do personagem.

**Análise de risco**  
Valor: 5 – Urgência: 4 – Risco: 2 – Esforço: 3 – Dependência: 4 – Prioridade: 18

**Protótipo relacionado a US**  
[Placeholder: imagem com opções de ação durante o turno]

## Épico 1.2: Posicionamento tático e alcance

### US03 - Definir espaços posicionais

**História de usuário**  
Como jogador, quero que o campo de batalha tenha posições com diferentes distâncias, para que o alcance dos ataques influencie as estratégias.

**Critérios de aceitação**  
- O campo de batalha deve exibir posições organizadas em distância (ex: perto, médio, longe).  
- Personagens e inimigos ocupam posições fixas ou móveis.  
- Cada posição influencia o alcance de habilidades.

**Regras de negócio**  
- O sistema deve associar cada ataque a um tipo de alcance (curto, médio, longo).  
- A movimentação consome o turno ou parte dele.

**Análise de risco**  
Valor: 4 – Urgência: 3 – Risco: 3 – Esforço: 4 – Dependência: 4 – Prioridade: 18

**Protótipo relacionado a US**  
[Placeholder: layout de campo com posições]

### US04 - Restringir alcance dos ataques

**História de usuário**  
Como jogador, quero que cada ataque só atinja inimigos nas posições permitidas, para tornar o posicionamento relevante no combate.

**Critérios de aceitação**  
- Cada ataque possui um raio ou distância definida.  
- O sistema impede execução de ataques fora do alcance.

**Regras de negócio**  
- O ataque é bloqueado se nenhum alvo válido estiver ao alcance.  
- Habilidades com múltiplos alvos devem respeitar o padrão de área.

**Análise de risco**  
Valor: 5 – Urgência: 4 – Risco: 3 – Esforço: 3 – Dependência: 3 – Prioridade: 18

**Protótipo relacionado a US**  
[Placeholder: imagem de seleção de alvo]

## Épico 1.3: Estratégias defensivas e interações táticas

### US05 - Enfrentar múltiplos inimigos

**História de usuário**  
Como jogador, quero enfrentar até quatro inimigos ou chefes maiores, para vivenciar batalhas desafiadoras e variadas.

**Critérios de aceitação**  
- O sistema deve suportar até quatro inimigos em tela simultaneamente.  
- Chefes ocupam mais espaço, mas equivalem a múltiplos inimigos.

**Regras de negócio**  
- O limite é imposto pela capacidade do cenário e regras do encontro.  
- Chefes podem ignorar algumas limitações de espaço.

**Análise de risco**  
Valor: 4 – Urgência: 4 – Risco: 2 – Esforço: 2 – Dependência: 2 – Prioridade: 14

**Protótipo relacionado a US**  
[Placeholder: imagem de chefes e múltiplos inimigos]

### US06 - Executar ataques inimigos

**História de usuário**  
Como jogador, quero que os inimigos ataquem com diferentes padrões, para adaptar minha defesa conforme o tipo de ataque.

**Critérios de aceitação**  
- Cada inimigo possui um conjunto distinto de ataques.  
- Os padrões devem variar entre ataques em linha, área e alvo único.

**Regras de negócio**  
- Ataques inimigos devem obedecer ao tempo de recarga (cooldown).  
- O sistema pode antecipar ataques por animação ou marcação.

**Análise de risco**  
Valor: 5 – Urgência: 4 – Risco: 3 – Esforço: 3 – Dependência: 4 – Prioridade: 19

**Protótipo relacionado a US**  
[Placeholder: imagem de padrão de ataque inimigo]

### US07 - Exibir área de ataque inimigo

**História de usuário**  
Como jogador, quero ver os espaços que serão atingidos pelos ataques inimigos, para reorganizar meus personagens e evitar dano.

**Critérios de aceitação**  
- O sistema deve exibir visualmente a área de impacto antes da execução.  
- A visualização deve ocorrer ao menos um turno antes.

**Regras de negócio**  
- Apenas inimigos com ataques previsíveis devem exibir essa informação.  
- A habilidade de percepção pode afetar essa visualização.

**Análise de risco**  
Valor: 5 – Urgência: 4 – Risco: 3 – Esforço: 3 – Dependência: 4 – Prioridade: 19

**Protótipo relacionado a US**  
[Placeholder: imagem da área de ataque]

### US08 - Alterar posições em combate

**História de usuário**  
Como jogador, quero reposicionar meus personagens durante o ataque inimigo, para proteger aliados vulneráveis ou ativar reações defensivas.

**Critérios de aceitação**  
- Deve haver uma fase de reposicionamento entre turnos inimigos.  
- A troca de posição deve obedecer às limitações de movimento.

**Regras de negócio**  
- O sistema pode limitar o número de trocas por rodada.  
- Trocas entre posições distantes podem ser proibidas ou custar mais.

**Análise de risco**  
Valor: 4 – Urgência: 4 – Risco: 3 – Esforço: 3 – Dependência: 3 – Prioridade: 17

**Protótipo relacionado a US**  
[Placeholder: animação de troca de posição]

### US09 - Ativar habilidades defensivas

**História de usuário**  
Como jogador, quero ativar parry, desvio ou bloqueio conforme o personagem em posição correta, para responder estrategicamente ao ataque inimigo.

**Critérios de aceitação**  
- As habilidades defensivas devem estar disponíveis apenas em determinadas posições.  
- O jogador deve poder escolher a resposta antes da execução do ataque inimigo.

**Regras de negócio**  
- Cada personagem possui um conjunto limitado de habilidades defensivas.  
- As habilidades têm cooldown e condições para uso.

**Análise de risco**  
Valor: 5 – Urgência: 5 – Risco: 3 – Esforço: 4 – Dependência: 4 – Prioridade: 21

**Protótipo relacionado a US**  
[Placeholder: imagem das reações defensivas]

### US10 - Usar habilidades com múltiplos alvos

**História de usuário**  
Como jogador, quero que habilidades atinjam diferentes espaços, para adaptar o uso conforme a formação inimiga.

**Critérios de aceitação**  
- O sistema deve permitir configurar padrões de área (linha, cone, círculo).  
- O jogador deve ver visualmente a área de efeito antes de confirmar.

**Regras de negócio**  
- A área de efeito é limitada por recursos, cooldown e tipo de habilidade.  
- Aliados podem ser atingidos se estiverem na área.

**Análise de risco**  
Valor: 4 – Urgência: 4 – Risco: 3 – Esforço: 3 – Dependência: 3 – Prioridade: 17

**Protótipo relacionado a US**  
[Placeholder: área de múltiplos alvos]

## Épico 1.4: Mecânicas especiais de combate

### US11 - Ativar preparo de combo

**História de usuário**  
Como jogador, quero ativar uma mecânica especial quando todos os aliados prepararem, para desbloquear ataques em grupo.

**Critérios de aceitação**  
- Cada aliado deve executar a ação de preparo em seu turno.  
- Após a preparação total, a opção de combo deve aparecer no menu.

**Regras de negócio**  
- A preparação é perdida se algum personagem for interrompido.  
- O combo consome todos os turnos seguintes.

**Análise de risco**  
Valor: 5 – Urgência: 5 – Risco: 3 – Esforço: 4 – Dependência: 5 – Prioridade: 22

**Protótipo relacionado a US**  
[Placeholder: barra de combo]

### US12 - Executar roleta de dano

**História de usuário**  
Como jogador, quero uma roleta como no *Dead by Daylight*, para causar dano máximo durante o combo.

**Critérios de aceitação**  
- O sistema exibe uma roleta interativa no momento do ataque em grupo.  
- A precisão do clique determina o multiplicador de dano.

**Regras de negócio**  
- A roleta tem área ideal que maximiza o dano.  
- O tempo para ativação é limitado.

**Análise de risco**  
Valor: 4 – Urgência: 3 – Risco: 2 – Esforço: 3 – Dependência: 3 – Prioridade: 15

**Protótipo relacionado a US**  
[Placeholder: imagem da roleta de precisão]
