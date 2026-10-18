# Decisões e trade-offs na Forge 25-Grid

[← Os 25 Domínios](03-os-25-dominios.md) · [Índice da documentação](README.md) · Próximo: [Framework de Cenários →](05-framework-de-cenarios.md)

---

A Forge 25-Grid não foi criada apenas para classificar áreas de uma empresa. Ela existe para tornar **decisões de negócio visíveis como trocas entre diferentes partes do sistema**.

A pergunta central não é apenas:

> Esta é uma boa decisão?

Mas sim:

> **O que esta decisão fortalece, o que ela enfraquece e qual é o custo escondido da escolha?**

Esse princípio é a ponte entre a grid como modelo de gestão e o **Grid Clash** como ambiente de prática.

## Uma decisão raramente afeta uma única célula

Uma decisão concreta costuma gerar vários efeitos ao mesmo tempo. Por exemplo, instalar caixas de autoatendimento pode aumentar a **Capacidade Operacional (O1)** e a **Lucratividade (F4)**, mas também reduzir o **Rigor (I4)** de controles antifraude e a **Atratividade (C3)** para clientes que valorizam atendimento humano.

A grid torna esse desenho explícito.

Cada efeito é representado como um impacto em um domínio:

- `+` — fortalece o domínio;
- `−` — cobra um custo ou enfraquece o domínio.

O objetivo não é eliminar trade-offs. **Bons gestores reconhecem e administram trade-offs.**

## A anatomia de uma decisão

Para modelar uma decisão com rigor, usamos quatro níveis:

```text
Ação ──produz──▶ Saída ──provoca──▶ Transformação
                                      │
                                 avaliada como
                                      ▼
                                  Resultado
                           (célula da grid + sinal)
```

### Ação

É aquilo que a empresa efetivamente faz.

Deve ser concreta e executável.

**Fraco:** “melhorar as vendas”.

**Forte:** “implantar reposição de estoque por ponto de pedido usando dados do PDV”.

### Saída

É o que a ação produz diretamente: um contrato, uma fila, um relatório, uma equipe treinada, um novo processo, um estoque adicional.

### Transformação

É a mudança de estado causada por essa saída: menos desperdício, maior capacidade de atendimento, mais capital imobilizado, menor tempo de espera, mais horas da equipe consumidas.

### Resultado

É a transformação interpretada do ponto de vista do negócio e associada a **uma célula da Forge 25-Grid**.

Um resultado sempre responde a duas perguntas:

1. **Qual domínio foi alterado?**
2. **O efeito ajuda (`+`) ou representa um custo/trade-off (`−`)?**

## Efeitos diretos e efeitos em cadeia

Nem todos os impactos acontecem no mesmo nível.

**Efeito de primeira ordem** é uma consequência direta da decisão.

> Comprar um segundo forno aumenta diretamente a **Capacidade Operacional (O1)**.

**Efeito de segunda ordem** aparece porque o primeiro efeito desencadeia outra mudança.

> O investimento no forno reduz o dinheiro disponível no curto prazo, afetando a **Liquidez (F2)**.

Uma boa análise considera os dois.

## Papel de cada impacto

Em cenários e exercícios, cada impacto pode assumir um papel:

- **primário** — o principal benefício pretendido pela decisão;
- **secundário** — um benefício adicional ou efeito em cadeia;
- **trade-off** — o preço pago pela decisão.

Uma decisão bem modelada normalmente contém mais de um impacto e pelo menos um custo relevante.

## O princípio pedagógico

O Grid Clash transforma esse raciocínio em prática repetida. O jogador recebe uma decisão e precisa identificar quais partes da grid serão afetadas.

A aprendizagem acontece quando a resposta é revelada e o jogador percebe:

- qual era o benefício óbvio;
- qual era o custo escondido;
- quais efeitos estavam em outro pilar;
- qual domínio foi ignorado na primeira leitura.

A lição central é simples:

> **Uma boa decisão de negócio ainda pode prejudicar outra parte do negócio.**

A grid não elimina essa tensão. Ela dá uma linguagem para enxergá-la, discuti-la e administrá-la.

---

Próximo: [Framework de Cenários →](05-framework-de-cenarios.md)
