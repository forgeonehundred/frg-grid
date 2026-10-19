# 🛒 Caixas de Autoatendimento

[← Índice de exemplos](README.md) · [Voltar ao README](../../../README.pt-BR.md)

*Cenário: **Supermercado** · decisão 3*

---

## A decisão

> A loja **substitui vários caixas com atendentes por totens de autoatendimento**.

É uma decisão clássica de eficiência — e um exemplo claro de trade-off entre domínios.

![Autoatendimento mapeado na grid](../../../assets/example-selfcheckout.svg)

## Célula por célula

| Célula | | Papel | peso | Por quê |
|---|---|---|---|---|
| **O1 Capacidade Operacional** | 🟩 + | primary | 1.0 | Mais pontos de checkout funcionam ao mesmo tempo no mesmo espaço físico, aumentando o volume atendido. |
| **F4 Lucratividade** | 🟩 + | primary | 1.0 | Menos horas de operadores por transação significam maior margem retida em cada venda. |
| **P4 Aproveitamento** | 🟩 + | secondary | 0.8 | Como efeito indireto, pessoas antes presas aos caixas podem ser realocadas para reposição e atendimento, aumentando o uso produtivo do tempo. |
| **I4 Rigor** | 🟥 − | tradeoff | 1.0 | Menos supervisão humana enfraquece controles de prevenção de perdas incorporados à rotina. |
| **C3 Atratividade** | 🟥 − | tradeoff | 1.0 | Uma experiência mais impessoal reduz a preferência de clientes que valorizam assistência humana. |

## O que isso mostra sobre a grid

- **Os ganhos se concentram; os custos se espalham.** Os ganhos aparecem em
  **Operações** (O1) e **Finanças** (F4), com um benefício adicional em **Pessoas**
  (P4). Já os custos atingem **Integridade** (I4) e **Comércio** (C3).
- **Integridade é fácil de esquecer.** O risco de perdas representado por I4 é
  justamente um dos efeitos que decisões desse tipo costumam ignorar. A grid o
  torna explícito.
- **O custo para a proposta de valor é real.** C3 Atratividade captura os clientes
  que valorizavam a presença de alguém no atendimento. Uma análise puramente de
  custo poderia deixar esse efeito invisível.

> **Aprendizado:** “autoatendimento reduz custos” pode ser verdade e ainda assim
> estar incompleto. A grid mostra uma troca entre ganhos de **Operações + Finanças**
> e custos em **Integridade + Comércio** — o que naturalmente leva a perguntas
> sobre prevenção de perdas e sobre o perfil de cliente que valoriza atendimento.

---

[← Anterior: 🍽️ Registro Contábil Diário](registro-contabil-diario.md) · Próximo exemplo: [🍏 Reduzir a Linha de Produtos →](linha-de-produtos-jobs.md)
