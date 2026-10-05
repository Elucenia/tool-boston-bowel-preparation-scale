<!-- ELUCENIA technical documentation · boston-bowel-preparation-scale · it · no clinical/professional/rights approval -->

# Scala di preparazione intestinale di Boston (BBPS)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/boston-bowel-preparation-scale)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Colon destro (cieco e ascendente)

`dir`

- `0` — 0 – Mucosa non visibile (feci solide)
- `1` — 1 – Parte della mucosa visibile
- `2` — 2 – Residuo minimo, mucosa ben visibile
- `3` — 3 – Tutta la mucosa ben visibile

### Colon trasverso (flessure incluse)

`trans`

- `0` — 0 – Mucosa non visibile (feci solide)
- `1` — 1 – Parte della mucosa visibile
- `2` — 2 – Residuo minimo, mucosa ben visibile
- `3` — 3 – Tutta la mucosa ben visibile

### Colon sinistro (discendente, sigma e retto)

`esq`

- `0` — 0 – Mucosa non visibile (feci solide)
- `1` — 1 – Parte della mucosa visibile
- `2` — 2 – Residuo minimo, mucosa ben visibile
- `3` — 3 – Tutta la mucosa ben visibile

## Edizione del metodo

BBPS/Lai 2009: 3 segmenti 0–3 dopo lavaggio/aspirazione; totale 0–9

## Formula documentata

Ogni segmento riceve 0 a 3 dopo lavaggio e aspirazione:

0: non preparato; mucosa nascosta da feci solide non rimovibili.

1: parte visibile, altre aree coperte da macchie, feci residue o liquido opaco.

2: piccoli residui, mucosa ben visibile.

3: tutta la mucosa visibile, senza residui.

Totale 0 a 9.

## Limiti e popolazione

La BBPS è stata sviluppata per assegnare un punteggio alla pulizia osservata durante l’ispezione dopo lavaggio e aspirazione da parte dell’endoscopista. Lo studio originale monocentrico non conferma automaticamente le soglie di adeguatezza o gli intervalli di ripetizione adottati in raccomandazioni successive. La valutazione di ogni segmento e l’edizione di questi criteri devono essere preservate.

## Riferimenti

- [Lai EJ et al. The Boston bowel preparation scale: a valid and reliable instrument for colonoscopy-oriented research. Gastrointest Endosc, 2009.](https://doi.org/10.1016/j.gie.2008.05.057)

- [Calderwood AH, Jacobson BC. Comprehensive validation of the Boston Bowel Preparation Scale. Gastrointest Endosc, 2010.](https://doi.org/10.1016/j.gie.2010.06.068)

- [Johnson DA et al. Optimizing adequacy of bowel cleansing for colonoscopy: recommendations from the US Multi-Society Task Force on Colorectal Cancer. Gastroenterology, 2014.](https://doi.org/10.1053/j.gastro.2014.07.002)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
