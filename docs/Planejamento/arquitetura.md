# Arquitetura do Projeto Unity

## Objetivo

Este documento tem como objetivo descrever a estrutura organizacional do projeto **Filho do Destino** na Unity, incluindo a hierarquia de pastas, convenções de código, utilização de prefabs, organização das cenas e padrões de desenvolvimento adotados pela equipe.

---

## Estrutura de Pastas

A estrutura a seguir é adotada dentro da pasta `Assets/` do projeto:

```title="Diagrama de Pastas"
Assets/
│
├── _Project/               # Arquivos específicos do projeto (configurações, cenas principais)
│   ├── Scenes/             # Cenas principais do jogo
│   ├── ScriptableObjects/  # Dados do jogo configuráveis
│   ├── Resources/          # Assets acessados via código em tempo de execução
│
├── Art/                    # Assets visuais
│   ├── Sprites/            # Sprites gerais
│   ├── Characters/         # Sprites dos personagens
│   ├── Anim/               # Animações dos personagens
│   ├── Tilesets/           # Tiles para mapas
│   ├── UI/                 # Imagens de interface
│
├── Audio/                  # Sons e músicas
│   ├── SFX/                # Efeitos sonoros
│   ├── Music/              # Trilha sonora
│
├── Prefabs/                # Prefabs prontos para instanciar
│   ├── Characters/         # Jogadores e inimigos
│   ├── UI/                 # Interfaces e HUDs
│
├── Scripts/                # Códigos fonte do jogo
│   ├── Core/               # Scripts principais (GameManager, InputManager, etc.)
│   ├── Combat/             # Scripts relacionados ao sistema de combate
│   ├── Characters/         # Scripts dos semideuses e inimigos
│   ├── UI/                 # Scripts de interface
│   ├── Dialogue/           # Scripts do sistema de diálogo
│
├── Animations/             # Animações .anim e controladores .controller
│   ├── Characters/         # Animações por personagem
│
├── Fonts/                  # Tipografias utilizadas no projeto
├── Materials/              # Materiais utilizados
├── Plugins/                # Assets externos/plugins
```

---

## Organização de Cenas

| Cena               | Função                                     |
|--------------------|--------------------------------------------|
| `MainMenu.unity`   | Tela inicial do jogo (botões, configurações) |
| `Overworld.unity`  | Área de exploração (sem combate)            |
| `Combat.unity`     | Cena de combate tático por turnos          |
| `DialogueTest.unity` | Cena de testes de narrativa e diálogos   |

---

## Uso de Prefabs

- Cada semideus tem um **prefab individual** com seus componentes (animação, stats, habilidades).
- Inimigos também são organizados em prefabs reutilizáveis.
- **UI modularizada** em prefabs: HUD, barra de vida, botões de ação, janela de diálogo.
- Todos os prefabs ficam em: `Assets/Prefabs/`

---

## ScriptableObjects

Usados para armazenar dados de forma modular e reutilizável:

| Tipo                     | Local                          | Função                         |
|--------------------------|--------------------------------|--------------------------------|
| `HabilidadeSO`           | `ScriptableObjects/Habilidades` | Dados de habilidades dos personagens |
| `PersonagemSO`           | `ScriptableObjects/Personagens` | Informações dos semideuses     |
| `InimigoSO`              | `ScriptableObjects/Inimigos`    | Atributos e fraquezas dos inimigos |
| `ConfigCombateSO`        | `ScriptableObjects/Combate`     | Configurações globais do sistema de combate |

---

## Convenções de Código

- **Nomenclatura PascalCase** para classes, métodos e propriedades públicas.
- **camelCase** para variáveis privadas.
- Arquivos de script seguem o padrão `NomeFuncionalidadeManager`, `TipoSistemaController`, etc.
- Componentes obrigatórios são definidos com `[RequireComponent]`.
- Scripts centralizadores como `GameManager`, `CombatManager` e `UIManager` são Singleton ou adicionados via tag única na cena.

---

## Sistemas Modulares

| Sistema             | Descrição                                                |
|---------------------|----------------------------------------------------------|
| `GameManager`       | Controla estados globais do jogo                         |
| `CombatManager`     | Controla entrada e lógica de combate por turnos         |
| `TurnHandler`       | Controla ordem dos turnos baseada em velocidade          |
| `DialogueSystem`    | Gera falas interativas estilo Undertale                 |
| `CharacterController` | Controla entrada de movimento dos personagens           |
| `UIController`      | Atualiza elementos visuais da interface (HUD, textos)   |
| `HabilityController`      | Controla a habilidade dos personagens e sua arvore   |

---

## Observações Finais

- Toda arte é criada em **Aseprite** e exportada como `.png`.
- Utilizamos **Unity URP (2D)** para renderização leve e personalizável.
- Organização do projeto busca facilitar manutenção, testes, e separação clara entre lógica, arte e dados.

---

## Histórico de Versões

| Versão | Data       | Descrição                       | Autor                           | Revisor                      |
|--------|------------|----------------------------------|----------------------------------|------------------------------|
| 1.0    | 10/07/2025 | Estrutura inicial do documento  | [João Vitor Merlin](https://github.com/jvopBR) | [Gabriel Sampaio](https://github.com/Faehzin) |

