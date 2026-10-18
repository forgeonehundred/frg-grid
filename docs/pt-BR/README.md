# Documentação da Forge 25-Grid — PT-BR

[← Voltar ao README principal](../../README.pt-BR.md)

---

Esta documentação reúne em uma única sequência o **modelo da Forge 25-Grid**, a lógica de **decisões e trade-offs**, o método para **criação de cenários** e a aplicação prática no **Forge Dojo: Grid Clash**.

A organização foi pensada para leitura progressiva: primeiro entender a estrutura do modelo, depois como decisões movimentam a grid e, por fim, como esse raciocínio vira prática e conteúdo jogável.

## Trilha recomendada

### 1. [A Grid](01-a-grid.md)

Como funciona o modelo 5×5, o significado dos dois eixos e como ler os códigos das células.

### 2. [Os Cinco Pilares](02-os-cinco-pilares.md)

As cinco grandes áreas do negócio: Comércio, Operações, Pessoas, Finanças e Integridade.

### 3. [Os 25 Domínios](03-os-25-dominios.md)

Referência completa de cada célula da grid, com definição e exemplos do que ela representa.

### 4. [Decisões e trade-offs](04-decisoes-e-tradeoffs.md)

Como uma decisão real produz efeitos em várias partes do negócio e por que bons movimentos ainda podem cobrar um preço em outras células.

### 5. [Framework de criação de cenários](05-framework-de-cenarios.md)

Método rigoroso para transformar decisões concretas em Ações, Saídas, Transformações e Resultados mapeados na Forge 25-Grid.

### 6. [Forge Dojo: Grid Clash](06-grid-clash.md)

Como o modelo vira uma experiência prática de aprendizagem baseada em decisões, votação, revelação e discussão de trade-offs.

### 7. [Exemplos](examples/)

Casos concretos de decisões mapeadas célula por célula.

---

## Como as partes se conectam

```text
Forge 25-Grid
   │
   ├── estrutura do negócio
   │      ├── 5 pilares
   │      └── 5 dimensões
   │
   ├── 25 domínios
   │
   ├── decisões
   │      ├── benefícios
   │      ├── efeitos secundários
   │      └── trade-offs
   │
   ├── cenários
   │      └── Ação → Saída → Transformação → Resultado
   │
   └── Grid Clash
          └── prática repetida de leitura de decisões
```

O objetivo é que a grid funcione como uma **linguagem comum de gestão**. Os cenários e o jogo existem para treinar essa linguagem em decisões concretas.

## Sobre a adaptação brasileira

Esta versão não é uma tradução literal dos termos em inglês. Os nomes foram ajustados para soar naturais em português brasileiro e funcionar como **estados ou recursos controláveis do negócio**.

Exemplos:

- `Availability` → **Prontidão**
- `Capacity` → **Capacidade Operacional**
- `Responsiveness` → **Agilidade**
- `Desirability` → **Atratividade**
- `Workforce` → **Equipe**
- `ROI` → **Retorno**

O código das células (`C1`, `O4`, `F2` etc.) permanece igual, preservando compatibilidade conceitual com a versão original.
