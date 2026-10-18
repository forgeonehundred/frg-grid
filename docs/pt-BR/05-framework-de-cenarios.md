# Framework de criação de cenários

[← Decisões e trade-offs](04-decisoes-e-tradeoffs.md) · [Índice da documentação](README.md) · Próximo: [Grid Clash →](06-grid-clash.md)

---

Este é o método de referência para construir cenários da Forge 25-Grid com rigor. Ele adapta o pipeline de modelagem usado no `jel-scenario` para o formato de cenários do Grid Clash.

O objetivo é evitar mapeamentos arbitrários. Uma decisão não deve ser ligada a uma célula porque “parece fazer sentido”; o vínculo precisa ser derivado de uma cadeia causal clara e justificável pela definição do domínio.

## Fundamentos

Antes de escrever um cenário, considere três elementos:

- **a Forge 25-Grid** — 5 pilares × 5 dimensões = 25 domínios;
- **o catálogo de domínios** — cada célula possui uma definição precisa e exemplos;
- **o modelo causal de decisão** — Ação → Saída → Transformação → Resultado.

Na versão brasileira desta documentação, os pilares são:

- **C · Comércio**
- **O · Operações**
- **P · Pessoas**
- **F · Finanças**
- **I · Integridade**

E as dimensões são:

1. **Prontidão**
2. **Adaptabilidade**
3. **Eficácia**
4. **Eficiência**
5. **Sustentabilidade**

Um código de célula segue o formato `<pilar><dimensão>`, como `O4`, `P1`, `C2`, `F3` ou `I5`.

## O que é um cenário

Um cenário é uma narrativa de negócio decomposta em decisões concretas e seus efeitos.

```text
Ação ──produz──▶ Saída ──provoca──▶ Transformação
                                      │
                                 avaliada como
                                      ▼
                                  Resultado
                           (célula da grid + sinal)
```

### Ação

É algo concreto e procedural que a empresa faz. No Grid Clash, **uma Ação corresponde a uma decisão**.

Exemplo:

> Implantar um sistema de reposição baseado no ponto de pedido do PDV.

Evite formulações abstratas como “melhorar vendas”, “ser mais eficiente” ou “fortalecer a equipe”.

### Saída

É o que a ação produz diretamente: um relatório, um contrato, uma fila, uma nova rotina, uma equipe treinada, um estoque ou uma infraestrutura.

### Transformação

É a mudança de estado provocada pela saída: menos desperdício, menor tempo de espera, maior estoque disponível, menor flexibilidade financeira, mais horas de gestão consumidas.

### Resultado

É a transformação interpretada do ponto de vista do negócio e associada a uma célula da grid.

Cada resultado deve indicar:

- a célula afetada;
- se o efeito ajuda (`+`) ou representa um custo/trade-off (`−`);
- se é de primeira ordem ou de segunda ordem;
- o papel do efeito na decisão.

## Processo de criação

### 1. Defina o contexto

Descreva o negócio, os principais envolvidos e a realidade operacional em uma ou duas frases.

O contexto deve ser suficiente para que a decisão faça sentido sem exigir conhecimento externo.

### 2. Enumere ações concretas

Liste aproximadamente 16–20 decisões realistas que o operador poderia tomar.

Cada decisão deve ser específica e executável.

**Evite:**

> Melhorar o atendimento.

**Prefira:**

> Criar uma escala extra de atendimento nos horários de pico.

### 3. Modele Saídas → Transformações

Para cada ação, descreva:

- o que ela produz;
- quais mudanças de estado ela provoca;
- quais efeitos desconfortáveis ou custos aparecem junto com o benefício.

É aqui que está a maior parte do rigor do cenário.

### 4. Derive os resultados

Converta cada transformação em um resultado na grid.

Para cada resultado:

1. determine se é de **primeira ordem** ou **segunda ordem**;
2. classifique como benefício (`+`) ou trade-off (`−`);
3. associe a exatamente **uma célula** da grid;
4. justifique o mapeamento usando a definição do domínio.

O mapeamento deve ser defensável conceitualmente, não intuitivo apenas.

### 5. Atribua papel e peso

Use os seguintes papéis:

- `primary` — um dos 1–2 principais efeitos positivos;
- `secondary` — benefício adicional ou efeito positivo em cadeia;
- `tradeoff` — todo efeito negativo relevante.

Como referência:

- peso `1` para impactos primários;
- cerca de `0.8` para efeitos secundários ou de segunda ordem.

Os pesos são uma ferramenta de modelagem, não um substituto para a qualidade do raciocínio causal.

### 6. Escreva a justificativa pedagógica

A justificativa deve explicar, em uma ou duas frases:

- qual é o ganho principal;
- qual é o custo escondido;
- por que a decisão cria um trade-off relevante.

O texto deve ensinar a leitura da grid sem parecer uma aula teórica.

### 7. Registre a origem

Quando o cenário vier de um grafo de conhecimento ou modelo anterior, registre a referência de origem. Quando for criado diretamente, identifique-o como conteúdo manual.

Isso ajuda a manter rastreabilidade entre a decisão, a modelagem causal e o cenário jogável.

## Invariantes de qualidade

Um cenário não está pronto até atender a todos estes critérios:

- cada decisão afeta **3–6 células**;
- cada decisão possui pelo menos um trade-off `−`;
- toda célula é um código válido da Forge 25-Grid;
- todo impacto possui célula, sinal, peso, papel e explicação;
- a explicação é compatível com a definição do domínio;
- há mistura de efeitos de primeira e segunda ordem;
- as decisões são concretas e realistas;
- os efeitos não são mapeados “por sensação”.

## Exemplo resumido

### Decisão

> O restaurante compra um segundo forno para atender mais pedidos no horário de pico.

### Saídas

- novo equipamento instalado;
- maior capacidade simultânea de produção;
- saída relevante de caixa.

### Transformações

- mais pedidos podem ser preparados ao mesmo tempo;
- parte dos recursos financeiros deixa de estar disponível no curto prazo.

### Resultados

- `O1 Capacidade Operacional` `+` — efeito primário;
- `F2 Liquidez` `−` — trade-off.

O ponto não é dizer que comprar o forno é “certo” ou “errado”. O ponto é tornar explícito **o que se ganha e o que se sacrifica**.

## Formato de saída

No Grid Clash, cada cenário é materializado como um arquivo JSON contendo:

- metadados do cenário;
- lista ordenada de decisões;
- prompt de cada decisão;
- células impactadas;
- sinal, peso e papel de cada impacto;
- explicação de cada impacto;
- justificativa pedagógica.

A documentação de produto do Grid Clash descreve como esse conteúdo é consumido durante o jogo.

---

Próximo: [Grid Clash →](06-grid-clash.md)
