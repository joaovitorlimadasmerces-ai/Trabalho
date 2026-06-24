# Sistema de IA

A IA do **Escape Rush** será responsável por controlar NPCs amigáveis e inimigos, tornando as partidas mais dinâmicas e desafiadoras.

## NPCs Amigáveis

Os NPCs amigáveis ajudam o jogador durante a corrida:

### Guia
- Indica o caminho correto para o objetivo.

### Entregador de Buffs
- Fornece bônus temporários.
- Exemplo: aumento de velocidade por alguns segundos.

### Resgatador
- Salva o jogador uma única vez em situações específicas.

---

## NPCs Inimigos

Os NPCs inimigos criam obstáculos e aumentam a dificuldade da partida.

### Corredor Rival
- Compete diretamente com o jogador até o final da fase.

### Empurrador
- Tenta derrubar o jogador dos obstáculos.

### Guardião
- Bloqueia passagens estratégicas.
- Atrasa o avanço do jogador.

---

## Comportamento da IA

Os NPCs utilizarão um sistema de máquina de estados finitos (**FSM - Finite State Machine**), alternando entre os seguintes estados:

| Estado | Descrição |
|----------|----------|
| Idle | NPC permanece parado. |
| Patrol | NPC patrulha uma área definida. |
| Follow | NPC segue o jogador. |
| Interact | NPC realiza uma interação específica. |

### Detecção do Jogador

A identificação do jogador será realizada por:

- **Distância** (raio de alcance).
- **Linha de Visão** (*Raycast*).

---

## Implementação no Roblox Studio

### Ferramentas Principais

- **PathfindingService**
  - Responsável pela navegação e movimentação inteligente dos NPCs.

- **Humanoid**
  - Controle de movimentação e animações dos NPCs.

- **Raycast**
  - Utilizado para detecção de obstáculos e linha de visão.

- **RemoteEvents**
  - Comunicação entre servidor e cliente.

---

## Escopo Inicial (MVP)

Na primeira versão do sistema serão implementados apenas:

### NPC Amigável
- Entregador de Buffs

### NPC Inimigo
- Corredor Rival

### Funcionalidades Básicas
- Sistema de movimentação.
- Sistema de detecção do jogador.
- Sistema de comportamento baseado em FSM.

---

## Atualizações Futuras

Os seguintes NPCs serão adicionados em versões posteriores:

- Guia
- Resgatador
- Empurrador
- Guardião

Além disso, novas mecânicas de IA e interações avançadas poderão ser incorporadas para aumentar a variedade e o desafio das partidas.
