+++
title = "Durante a aventura"
description = "Utilize esta página enquanto estiver na aventura."
date = 2021-05-01T08:00:00+00:00
updated = 2021-05-01T08:00:00+00:00
draft = false
weight = 2
sort_by = "weight"
template = "game/page.html"

[extra]
lead = 'Utilize esta página enquanto estiver na aventura.'
toc = true
top = false
+++

## Estrutura da rodada

Cada rodada possui três fases:

| Ordem | Fase                  | Descrição                                                                                                                                         |
| ----- | --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1     | Fase de Ação          | Cada herói tem um turno, realizando até duas ações.                                                                                               |
| 2     | Fase da Sombra        | Inimigos são ativados, a escuridão é resolvida (se necessário) e a ameaça aumenta – eventos de ameaça são ativados se a ameaça atingir um limite. |
| 3     | Fase de Reagrupamento | Todos os heróis restauram seu baralho de perícias e então examinam duas cartas.                                                                   |

## Ações

Um herói pode realizar duas ações durante seu turno. O herói pode realizar a mesma ação mais de uma vez ou duas ações diferentes:

| Ação      | Descrição                                                                                                |
| --------- | -------------------------------------------------------------------------------------------------------- |
| Ataque    | Ataque um inimigo em seu espaço. Se você tiver uma arma de alcance, você pode atacar um inimigo próximo. |
| Viajar    | Mova-se até duas vezes. O herói pode realizar sua segunda ação entre o primeiro e o segundo movimento.   |
| Interagir | Interaja com uma ficha em seu espaço.                                                                    |

## Restaurando o Baralho

O herói deve reiniciar seu baralho nestes momentos:

    - Durante fase do reagrupamento
    - Quando não restarem cartas no baralho
    - Quando um efeito o instruir a fazer isso

O herói restaura seu baralho, embaralhando sua pilha de descarte com quaisquer cartas restantes no seu baralho e colocando o novo baralho virado para baixo. Cartas preparadas não são embaralhadas no baralho.

## Modificadores de Ataque

| Modificador | Descrição                                                                                                   |
| ----------- | ----------------------------------------------------------------------------------------------------------- |
| Perfurar    | Esse ataque ignora a armadura do inimigo.                                                                   |
| Castigar    | Esse ataque ignora a feitiçaria do inimigo.                                                                 |
| Rachar      | Esse ataque reduz permanentemente a armadura do inimigo em uma unidade (antes de o golpe ser aplicado).     |
| Fender      | Todos os inimigos no grupo sofrem o número completo de golpes.                                              |
| Letal       | Se esse ataque reduzir a vida atual do inimigo pelo menos pela metade, ele é derrotado.                     |
| Atordoar    | Esse ataque esgota o grupo inimigo. Se o grupo for de elite, ele também não pode contra-atacar este ataque. |

## Palavras-chave

| Palavra-Chave             | Descrição                                                                                                                                                                                                                                                                                       |
| ------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Fazer Reconhecimento Em X | Causada por efeito. Revele X cartas do topo do seu baralho de perícias. Você pode preparar uma dessas cartas (coloque-a virada para cima embaixo da sua carta de herói). Então, coloque cada uma das cartas reveladas restantes no topo ou fundo do seu baralho de perícias, em qualquer ordem. |
| Golpear X                 | Durante um teste de ataque, você pode descartar uma carta que tenha a palavra-chave "Golpear X" e adicionar X golpes ao ataque.                                                                                                                                                                 |
| Defender X                | Quando você ou um herói em seu espaço forem sofrer dano ou medo, você pode descartar uma carta que tenha a palavra-chave "Defender X" para prevenir qualquer combinação de X pontos de dano e medo.                                                                                             |
| Correr X                  | Durante seu turno, você pode descartar uma carta que tenha a palavra-chave "Correr X" para se mover X espaços adicionais. Você pode realizar ações entre cada movimento.                                                                                                                        |
| Descansar X               | No final do seu turno, você pode descartar uma carta que tenha a palavra-chave "Descansar X" para descartar um número de cartas de dano ou medo viradas para baixo igual a X.                                                                                                                   |
| Esconder X                | Depois de realizar um teste, você pode descartar uma carta que tenha a palavra-chave “Se Esconder" para receber uma carta de vantagem "Escondido".                                                                                                                                              |
