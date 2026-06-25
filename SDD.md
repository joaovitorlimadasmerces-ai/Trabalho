# CORRIDA CONTRA O TEMPO 
# Sound Design Document (SDD)

**Plataforma:** Roblox Studio

---

# 1. Objetivo do Documento

Este documento descreve o design sonoro do jogo **Escape Rush**, detalhando o papel da música e dos efeitos sonoros (SFX) na experiência do jogador.

O SDD serve como referência para implementação e expansão do sistema de áudio no Roblox Studio.

---

# 2. Visão Geral da Proposta Sonora

O jogo possui uma proposta sonora dinâmica e orientada à tensão, coerente com sua natureza de corrida intensa (*Obby Runner*).

O áudio foi projetado para cumprir três funções principais:

| Função | Descrição |
|---------|-------------|
| **Urgência** | Reforçar a sensação de velocidade e pressão constante |
| **Feedback** | Resposta imediata às ações do jogador |
| **Clareza** | Indicar momentos críticos: perigo, erro e progresso |

Diferente de jogos mais calmos, aqui o som é essencial para transmitir pressão constante, acompanhando a dinâmica da **Zona de Perigo** em tempo real.

---

# 3. Objetivos do Áudio

- Sustentar uma ambientação de tensão crescente ao longo da corrida.
- Reforçar ações positivas, como a coleta de energéticos e passagem por checkpoints.
- Alertar o jogador sobre a aproximação da Zona de Perigo.
- Comunicar falhas (morte) de forma impactante e clara.
- Manter clareza sonora mesmo com gameplay rápida e cheia de elementos simultâneos.

---

# 4. Biblioteca de Áudio

## 4.1 Música

Trilha principal que acompanha o jogador durante a corrida.

| Arquivo / Link | Tipo | Função |
|---------------|------|---------|
| ▶ Ouvir no YouTube | Trilha de fundo | Ambientação principal da partida |

---

## 4.2 Efeitos Sonoros (SFX)

Sons de feedback acionados por eventos específicos durante o gameplay.

| Arquivo / Link | Tipo | Função |
|---------------|------|---------|
| sounds/checkpoint.wav[checkpoint.mp3](https://github.com/user-attachments/files/29334613/checkpoint.mp3)
 | SFX | Feedback de checkpoint |
| sounds/lob.wav | SFX | Música do lob inicial |
| sounds/death.wav [game over.mp3](https://github.com/user-attachments/files/29334715/game.over.mp3)
| SFX | Feedback de morte |

---

# 5. Papel de Cada Elemento Sonoro

## 🎵 Música de Fundo

A trilha principal acompanha o jogador durante toda a corrida, aumentando gradualmente a intensidade conforme o progresso.

### Objetivos

- Manter o ritmo da gameplay e o engajamento do jogador.
- Evitar sensação de vazio ou monotonia.
- Aumentar a tensão conforme o jogador avança no percurso.

---

## ⚠️ Música de Alerta

Ativada quando a Zona de Perigo está próxima do jogador.

### Objetivos

- Gerar urgência imediata e instintiva.
- Indicar risco sem depender apenas de elementos visuais.

---

## ⚡ Som de Energético

Disparado ao coletar um item de buff durante a corrida.

### Objetivos

- Fornecer feedback positivo imediato.
- Reforçar a sensação de ganho de vantagem e impulso.

---

## 🔴 Som da Zona de Perigo

Som contínuo ou pulsante quando a zona está próxima do jogador.

### Objetivos

- Criar pressão psicológica constante.
- Avisar o jogador sem que precise olhar para trás.

---

## 💀 Som de Morte

Reproduzido ao ser alcançado pela Zona de Perigo ou ao falhar em um obstáculo.

### Objetivos

- Marcar claramente o fim da tentativa.
- Gerar impacto imediato e memorável.

---

## ✅ Som de Checkpoint

Ativado ao alcançar um marco de progresso no percurso.

### Objetivos

- Indicar progresso e conquista parcial.
- Gerar sensação de segurança momentânea e alívio.

---

# 6. Fluxo Sonoro da Experiência

A experiência sonora acompanha cada etapa do jogo de forma sequencial:

| Etapa | Evento |
|---------|---------|
| **1** | Jogador entra no lobby — som ambiente leve ou silêncio |
| **2** | Ao iniciar a partida, a música principal começa |
| **3** | Durante a corrida, efeitos rápidos acompanham cada ação do jogador |
| **4** | Conforme a Zona de Perigo se aproxima, sons de alerta aumentam a tensão |
| **5** | Ao morrer, um som marcante encerra a tentativa com impacto |
| **6** | Retorno ao lobby — ciclo reinicia |

---

# 7. Diretrizes de Mixagem

Para garantir clareza sonora durante o gameplay acelerado:

- Efeitos (SFX) devem ser mais altos que a música de fundo.
- Som de perigo deve se destacar progressivamente à medida que a zona se aproxima.
- Música não deve competir com os alertas críticos.
- Evitar sobreposição excessiva de sons simultâneos.
- Sons de ação devem ser curtos e objetivos, sem delay perceptível.

---

# 8. Coerência Estética Sonora

O estilo sonoro de **Escape Rush** segue as seguintes diretrizes:

| Aspecto | Diretriz |
|----------|-----------|
| **Ritmo** | Sons rápidos e responsivos, alinhados ao gameplay |
| **Estilo** | Trilha eletrônica e dinâmica |
| **Foco** | Tensão e urgência acima de tudo |
| **Eficiência** | Pouca complexidade, alto impacto |

---

# 9. Limitações Atuais

Na versão atual do projeto, os seguintes recursos ainda não estão implementados:

- Variação musical por mapa ou fase.
- Efeitos sonoros no menu e interfaces.
- Sistema de controle de volume separado (música / SFX).
- Múltiplas camadas de ambientação sonora.
- Transições sonoras avançadas entre estados do jogo.

---

# 10. Melhorias Futuras Sugeridas

- Adicionar som de interface para cliques e navegação.
- Criar trilha específica para o lobby.
- Implementar controle separado de volume (música / SFX) nas configurações.
- Adicionar variação sonora conforme a velocidade do jogador aumenta.
- Incluir efeitos únicos para diferentes tipos de obstáculos.
- Melhorar transições sonoras entre os estados do jogo.

---

# 11. Resumo

O design sonoro de **CORRIDA CONTRA O TEMPO ** é focado em ritmo, urgência e feedback imediato.

A música sustenta a tensão ao longo da corrida, enquanto os efeitos sonoros guiam o jogador e reforçam cada ação importante.

Mesmo com escopo inicial simples, o sistema sonoro é eficaz e possui grande potencial de expansão. Ele contribui diretamente para a intensidade e fluidez da gameplay, sendo um componente indispensável da experiência do jogador.

