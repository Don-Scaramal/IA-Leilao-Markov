# IA-Leilao-Markov
Implementação de um Processo de Decisão de Markov (MDP) e Aprendizado por Reforço num ambiente simulado de leilões.

# Otimização de Lances em Leilões: Processo de Decisão de Markov (MDP) 🐎

Este repositório contém a modelação matemática e a simulação de um ambiente de leilão competitivo, desenvolvido no Google Colab, com foco na aplicação de conceitos de Aprendizado por Reforço e Processos de Decisão de Markov (MDP).

## 🎯 Objetivo do Projeto
O objetivo foi criar uma simulação iterativa onde um agente autónomo interage num leilão de ativos (neste cenário, cavalos de diferentes valores) contra um oponente com regras determinísticas de limite de orçamento. O projeto foca-se na extração e análise das recompensas obtidas ao longo de múltiplos episódios.

## ⚙️ Arquitetura do MDP
A lógica do leilão foi estruturada através dos princípios fundamentais de um Processo de Decisão de Markov:
*   **Estados:** Mapeamento contínuo do `item_atual`, `lance_atual`, `budget_agente` e `budget_oponente`.
*   **Ações:** O espaço de ação do agente é definido pela decisão binária de passar o turno ou aumentar o lance (com incrementos estáticos ou aleatórios).
*   **Recompensas:** Sistema de pontuação definido pelo valor real do item arrematado deduzido do custo do lance pago.
*   **Transições:** Geridas pelo ambiente virtual desenvolvido de raiz para a simulação.

## 🛠️ Tecnologias e Bibliotecas Utilizadas
*   **Python 3:** Linguagem base para desenvolvimento da lógica orientada a objetos (classes `Item`, `AgenteAleatorio`, `Oponente` e `AmbienteLeilao`).
*   **Numpy & Math:** Para cálculos numéricos e gestão de aleatoriedade nos lances e distribuições.
*   **Matplotlib:** Para a visualização e análise de dados gerados.

## 📊 Análise de Dados e Resultados
O código inclui a geração de um relatório de desempenho gráfico com avaliação direta entre o Agente e o Oponente, analisando:
1. Evolução do Património ao longo dos episódios.
2. Comparação de Recompensas Obtidas (lucro de arremate).
3. Volume de itens adquiridos por participante.
4. Saldo de caixa (budget) remanescente.

> *Projeto desenvolvido para exploração prática de arquiteturas de IA e otimização matemática.*
