# Trabalho
[EscapeRush_GDD_v1.0.docx.pdf](https://github.com/user-attachments/files/29204342/EscapeRush_GDD_v1.0.docx.pdf)
[EscapeRush_SDD_v1.0.docx.pdf](https://github.com/user-attachments/files/29204340/EscapeRush_SDD_v1.0.docx.pdf)

# 🎮 CORRIDA CONTRA O TEMPO — Documento de Design

## 1. Visão Geral do Projeto

**Escape Rush** é um jogo no estilo **Runner / Obstacle Course (Obby)** desenvolvido no Roblox Studio.

O objetivo central é avançar por um percurso linear repleto de obstáculos, alcançando o final da fase antes de ser eliminado por uma zona de perigo que persegue o jogador constantemente.

| Campo | Detalhe |
|------|--------|
| Nome Provisório | Escape Rush |
| Plataforma | Roblox Studio |
| Gênero | Runner / Obstacle Course (Obby) |
| Perspectiva | Terceira pessoa |
| Número de Jogadores | 1+ (multiplayer assíncrono) |
| Versão do Documento | 1.0 — Rascunho Inicial |

---

## 1.1 Proposta de Valor

Escape Rush combina:
- A simplicidade de um Obby clássico
- Com a tensão de uma zona de perigo em perseguição constante

Criando uma experiência:
- Urgente  
- Viciante  
- Estratégica  

---

## 2. Mecânicas de Jogo

### 2.1 Fluxo Principal

1. Lobby → Preparação e entrada na partida
2. Obstaculo → Partes tocaveis que morrem  
3. Corrida → Superar obstáculos  
4. Fim → Completar ou morrer  

---

### 2.2 Lobby

- Entrada automática ao iniciar ou morrer  
- Partida com tempo 
- Teleporte para o início do percurso  

Pode exibir:
- Estatísticas  
- Recordes  
- Cosméticos  

---

### 2.3 Corrida e Percurso

- Percurso linear
- Avanço contínuo

**Ações do jogador:**
- Correr  
- Pular  
- Desviar  

**Características:**
- Dificuldade progressiva  
- Segmentos variados  

**Exemplos de obstáculos:**
- Plataformas móveis  
- Armadilhas  
- Buracos
- NPC 

---

## 2.4 Zona de Perigo

Barreira que persegue o jogador ou NPC.

**Características:**
- Movimento constante ou crescente  

| Condição | Resultado |
|---------|----------|
| Encostar na zona | Morte instantânea |
| Respawn | Início ou checkpoint |

**Feedback:**
- Som de alerta  
- Efeitos visuais  

---

## 2.5 Sistema de Buffs

| Buff | Efeito | Duração |
|------|--------|--------|
| Energético | Aumenta velocidade | 5–10s |
| Escudo | Sobrevive 1 vez | Uso único |
| Super Salto | Aumenta pulo | 3–5s |
| Voo | Voa temporariamente  | 2-5s |


---

## 3. Estrutura de Fase

### 3.1 Segmentos

| Fase | Características |
|------|---------------|
| Início | Obstáculos simples |
| Meio | Plataformas móveis |
| Final | Alta velocidade |

---

### 3.2 Obstáculos

- Buracos  
- Plataformas móveis  
- Blocos caindo  
- Plataformas que somem  
- Corredores estreitos  

---

### 3.3 Condições

**Vitória:**
- Chegar ao final  

**Derrota:**
- Ser alcançado  
- Cair  

---

## 4. Experiência do Jogador

### 4.1 Pilares

- Urgência  
- Fluidez  
- Recompensa  
- Rejogabilidade  

---

### 4.2 Sensação

- Adrenalina constante  
- Pressão crescente  
- Satisfação ao escapar  

---

### 4.3 Feedback
 
- Sons de alerta  
- Efeitos de velocidade  
- Celebração final  

---

## 5. Considerações Técnicas

### 5.1 Arquitetura

- Movimento → LocalScript  
- Zona → Script no servidor  
- Buffs → Touched + RemoteEvent  
- Lobby → TeleportService  

---

### 5.2 Sistemas

| Sistema | Implementação |
|--------|--------------|
| Movimento | Humanoid |
| Zona | TweenService |
| Buffs | RemoteEvent |
| Chegada | Trigger |
| Lobby | TeleportService |
| Dados | DataStore |

---

## 6. Escopo

### 6.1 MVP

- 1 fase  
- Zona funcional  
- Buff de velocidade  
- Lobby  
- Tela de fim  

---

### 6.2 Futuro

- Novas fases  
- Dificuldades  
- Loja  
- Ranking  
- Multiplayer  
- Novos buffs  

---

### 6.3 Pendências

- Nome final  
- Velocidade da zona  
- Buffs  
- Tema visual  
- Checkpoints  

---

## 7. Glossário

| Termo | Definição |
|------|----------|
| Obby | Percurso de obstáculos |
| Runner | Jogo de corrida contínua |
| Zona de Perigo | Barreira perseguidora |
| Buff | Vantagem temporária |
| MVP | Versão mínima |
| Lobby | Área de espera |
| DataStore | Sistema de dados |
