<!-- ELUCENIA technical documentation · boston-bowel-preparation-scale · pt-BR · no clinical/professional/rights approval -->

# Escala de Boston (BBPS)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/boston-bowel-preparation-scale)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Cólon direito (ceco e ascendente)

`dir`

- `0` — 0 – mucosa não vista (fezes sólidas)
- `1` — 1 – parte da mucosa vista
- `2` — 2 – resíduo mínimo, mucosa bem vista
- `3` — 3 – toda a mucosa bem vista

### Cólon transverso (flexuras incluídas)

`trans`

- `0` — 0 – mucosa não vista (fezes sólidas)
- `1` — 1 – parte da mucosa vista
- `2` — 2 – resíduo mínimo, mucosa bem vista
- `3` — 3 – toda a mucosa bem vista

### Cólon esquerdo (descendente, sigmoide e reto)

`esq`

- `0` — 0 – mucosa não vista (fezes sólidas)
- `1` — 1 – parte da mucosa vista
- `2` — 2 – resíduo mínimo, mucosa bem vista
- `3` — 3 – toda a mucosa bem vista

## Edição do método

BBPS/Lai 2009:3 segmentos 0–3, após lavagem/aspiração, total 0–9

## Fórmula documentada

Cada segmento recebe de 0 a 3 após lavagem e aspiração:

0: segmento não preparado, mucosa não vista por fezes sólidas que não saem.

1: parte da mucosa vista; outras áreas encobertas por manchas, fezes residuais ou líquido opaco.

2: pequenos resíduos, mucosa bem vista.

3: toda a mucosa bem vista, sem resíduos.

Total de 0 a 9.

## Limites e população

A BBPS foi desenvolvida para pontuar a limpeza observada na inspeção após lavagem e aspiração pelo endoscopista. O estudo original de centro único não confirma automaticamente os cortes de adequação ou intervalos de repetição adotados em recomendações posteriores. A avaliação de cada segmento e a edição desses critérios devem ser preservadas.

## Referências

- [Lai EJ et al. The Boston bowel preparation scale: a valid and reliable instrument for colonoscopy-oriented research. Gastrointest Endosc, 2009.](https://doi.org/10.1016/j.gie.2008.05.057)

- [Calderwood AH, Jacobson BC. Comprehensive validation of the Boston Bowel Preparation Scale. Gastrointest Endosc, 2010.](https://doi.org/10.1016/j.gie.2010.06.068)

- [Johnson DA et al. Optimizing adequacy of bowel cleansing for colonoscopy: recommendations from the US Multi-Society Task Force on Colorectal Cancer. Gastroenterology, 2014.](https://doi.org/10.1053/j.gastro.2014.07.002)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

As informações abaixo preservam as saídas do método para exemplos sintéticos. Não constituem validação clínica independente.

### 1

Preparo adequado (total ≥ 6 e todos os segmentos ≥ 2)

| Detalhes do resultado | |
| --- | --- |
| Cólon direito | 3 |
| Cólon transverso | 3 |
| Cólon esquerdo | 3 |


### 2

Preparo adequado (total ≥ 6 e todos os segmentos ≥ 2)

| Detalhes do resultado | |
| --- | --- |
| Cólon direito | 2 |
| Cólon transverso | 2 |
| Cólon esquerdo | 2 |


### 3

Preparo inadequado: repetir a colonoscopia em intervalo curto

| Detalhes do resultado | |
| --- | --- |
| Cólon direito | 1 |
| Cólon transverso | 3 |
| Cólon esquerdo | 3 |

Total ≥ 6, mas há segmento com nota < 2: o preparo não é considerado adequado.


### 4

Preparo inadequado: repetir a colonoscopia em intervalo curto

| Detalhes do resultado | |
| --- | --- |
| Cólon direito | 1 |
| Cólon transverso | 1 |
| Cólon esquerdo | 1 |

