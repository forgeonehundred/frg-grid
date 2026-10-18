# Forge Dojo: Grid Clash

[← Framework de Cenários](05-framework-de-cenarios.md) · [Índice da documentação](README.md)

---

O **Forge Dojo: Grid Clash** é a aplicação prática da Forge 25-Grid em formato de jogo colaborativo.

Seu objetivo não é ensinar a grid por meio de aulas passivas. O aprendizado acontece pela repetição de decisões reais de negócio e pela comparação entre a leitura do jogador e os impactos mapeados no modelo.

## Princípio do produto

O Grid Clash é uma arena de prática.

A cada rodada, os jogadores recebem uma decisão de negócio e precisam responder:

> **Quais partes da Forge 25-Grid essa decisão afeta?**

Depois da votação, o jogo revela:

- quais células eram impactadas;
- quais impactos eram positivos;
- quais eram trade-offs;
- a justificativa por trás do mapeamento.

A principal lição é que uma decisão empresarial raramente é boa ou ruim de forma isolada. Ela redistribui forças e fragilidades pelo sistema.

## Estrutura de conteúdo

Um **cenário** é um conjunto jogável de decisões dentro de um contexto empresarial.

Exemplos:

- restaurante;
- supermercado;
- indústria;
- empresa de tecnologia;
- empresa em recuperação;
- operação em expansão.

Cada cenário contém várias **decisões**.

```text
Cenário
 ├── Decisão 1
 ├── Decisão 2
 ├── Decisão 3
 └── ...
```

Cada decisão possui:

- título;
- situação ou prompt;
- células impactadas;
- sinal de cada impacto (`+` ou `−`);
- peso;
- papel (`primary`, `secondary`, `tradeoff`);
- explicação;
- justificativa pedagógica.

## Como uma rodada funciona

Em uma rodada típica:

1. o jogo apresenta uma decisão;
2. cada jogador seleciona de 1 a 3 células que acredita serem afetadas;
3. as escolhas são registradas;
4. a resposta é revelada;
5. os impactos corretos aparecem na grid;
6. o jogo explica os benefícios e custos escondidos;
7. a pontuação é calculada.

O jogador não escolhe inicialmente se o impacto é positivo ou negativo. O sinal é revelado depois da votação para preservar o valor pedagógico da descoberta.

## O que a pontuação recompensa

A pontuação foi desenhada para incentivar três comportamentos:

- **precisão** — identificar as células corretas;
- **percepção de trade-offs** — encontrar custos que não são óbvios;
- **velocidade** — decidir com agilidade sem transformar a rodada em um teste de memorização.

Selecionar muitas células sem critério não é vantajoso. A proximidade é calculada sobre as células escolhidas pelo jogador, portanto palpites errados diluem a qualidade da resposta.

## Proximidade entre células

A grid também permite reconhecer respostas parcialmente corretas.

Uma seleção pode ser:

- **exata** — a célula correta;
- **próxima pelo pilar** — outra célula da mesma coluna;
- **próxima pela dimensão** — outra célula da mesma linha;
- **incorreta** — sem relação suficiente com a resposta esperada.

Isso reforça que a grid não é apenas uma lista de 25 nomes. Ela possui estrutura.

Por exemplo:

- `F4 Lucratividade` e `F2 Liquidez` compartilham o pilar **Finanças**;
- `O4 Eficiência Operacional` e `F4 Lucratividade` compartilham a dimensão **Eficiência**.

## Trade-offs como parte da resposta

Uma decisão pode ter várias células corretas.

Algumas representam benefícios pretendidos. Outras representam custos.

Exemplo:

> Automatizar parte do atendimento pode aumentar **O1 Capacidade Operacional** e **F4 Lucratividade**, mas reduzir **C3 Atratividade** para clientes que valorizam interação humana.

O jogo recompensa jogadores que identificam esses custos escondidos porque eles representam uma competência essencial de gestão: perceber efeitos que aparecem fora da área diretamente beneficiada.

## Visão de equipe

O Grid Clash também agrega as escolhas dos jogadores em uma leitura coletiva.

A distribuição de votos pode ser apresentada como um mapa de calor sobre a grid. Isso permite visualizar:

- onde existe consenso;
- quais células dividem a equipe;
- quais áreas foram ignoradas;
- quanto o grupo percebeu dos impactos secundários e trade-offs.

Nesse sentido, a grid funciona também como uma linguagem compartilhada para discussão de decisões.

## Papéis durante uma sessão

### Facilitador

O facilitador conduz a sessão, apresenta as decisões, controla o ritmo e revela as respostas.

Ele pode usar a discussão após cada rodada para explorar perguntas como:

- Por que vocês escolheram essa célula?
- Qual impacto parecia mais óbvio?
- Qual custo passou despercebido?
- Esse efeito é direto ou consequência de outro?
- Qual pilar ficou menos visível nesta decisão?

### Jogador

O jogador interpreta a situação, seleciona as células afetadas e compara seu raciocínio com o modelo revelado.

O objetivo não é memorizar respostas, mas desenvolver uma forma mais estruturada de enxergar negócios.

## O ciclo de aprendizagem

O Grid Clash usa um ciclo simples:

```text
Decisão
   ↓
Hipótese do jogador
   ↓
Mapeamento na grid
   ↓
Revelação
   ↓
Discussão do trade-off
   ↓
Nova decisão
```

Com repetição, os jogadores passam a reconhecer padrões entre diferentes tipos de negócio.

## Relação com o restante desta documentação

A documentação da Forge 25-Grid pode ser lida em três camadas:

1. **Modelo** — entender pilares, dimensões e os 25 domínios;
2. **Decisão** — entender como ações alteram múltiplas células e criam trade-offs;
3. **Prática** — aplicar esse raciocínio em cenários e sessões do Grid Clash.

Para construir novos cenários, consulte o [Framework de criação de cenários](05-framework-de-cenarios.md).

Para consultar o significado de cada célula, veja [Os 25 Domínios](03-os-25-dominios.md).

---

[← Framework de Cenários](05-framework-de-cenarios.md) · [Índice da documentação](README.md)
