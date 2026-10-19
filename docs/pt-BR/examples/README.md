# Exemplos

[← Os 25 Domínios](../03-os-25-dominios.md) · [Voltar ao README](../../../README.pt-BR.md)

---

É aqui que a grid ganha vida. Cada exemplo parte de **uma decisão real** —
retirada diretamente dos cenários de [Forge Dojo: Grid Clash](https://forge100.com) —
e mostra como seus efeitos aparecem no tabuleiro, célula por célula.

O padrão é sempre o mesmo, e ele resume a lógica do modelo:

> **Uma decisão quase nunca afeta uma única célula.** Ela fortalece alguns domínios
> (`+`), cobra um preço em outros (`−`) e o **trade-off entre eles é o aprendizado.**

Cada impacto em uma célula carrega três informações:

- um **sinal** — `+` fortalece o domínio; `−` enfraquece ou cobra um custo;
- um **papel** — `primary` (efeito principal pretendido), `secondary` (efeito
  indireto) ou `tradeoff` (o preço pago pela decisão);
- um **peso** (0–1) — a intensidade do efeito.

---

## Os exemplos

| Exemplo | Decisão | O trade-off em uma frase |
|---|---|---|
| [🍽️ Registro Contábil Diário](registro-contabil-diario.md) | Registrar todas as transações todos os dias | Visibilidade do lucro **vs.** tempo do gestor |
| [🛒 Caixas de Autoatendimento](autoatendimento.md) | Substituir caixas atendidos por totens | Capacidade e margem **vs.** controle e atendimento humano |
| [🍏 Reduzir a Linha de Produtos](linha-de-produtos-jobs.md) | Apple reduz ~350 produtos para 4 | Foco e liquidez **vs.** segmentos abandonados |

---

## Como ler os diagramas

Cada exemplo inclui uma mini-grid em que as células afetadas ficam destacadas:

- 🟩 **verde** = a decisão **fortalece** o domínio (`+`);
- 🟥 **vermelho** = a decisão **cobra um custo** naquele domínio (`−`);
- cinza = sem alteração.

O marcador em cada célula mostra o sinal, enquanto o papel e o peso aparecem na
parte inferior. Ao acompanhar verdes e vermelhos entre os **domínios**, fica fácil
ver quando uma decisão é, por exemplo, “boa para Finanças e Operações, mas paga
esse ganho com Pessoas”.

---

[← Os 25 Domínios](../03-os-25-dominios.md) · [Voltar ao README](../../../README.pt-BR.md)
