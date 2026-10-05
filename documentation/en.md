<!-- ELUCENIA technical documentation · boston-bowel-preparation-scale · en · no clinical/professional/rights approval -->

# Boston Bowel Preparation Scale (BBPS)

[conditions, sources and permissions](https://elucenia.org/en/tools/boston-bowel-preparation-scale)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Right colon (cecum and ascending colon)

`dir`

- `0` — 0 – Mucosa not seen (solid stool)
- `1` — 1 – Part of mucosa seen
- `2` — 2 – Minimal residue, mucosa clearly seen
- `3` — 3 – Entire mucosa clearly seen

### Transverse colon (including flexures)

`trans`

- `0` — 0 – Mucosa not seen (solid stool)
- `1` — 1 – Part of mucosa seen
- `2` — 2 – Minimal residue, mucosa clearly seen
- `3` — 3 – Entire mucosa clearly seen

### Left colon (descending, sigmoid and rectum)

`esq`

- `0` — 0 – Mucosa not seen (solid stool)
- `1` — 1 – Part of mucosa seen
- `2` — 2 – Minimal residue, mucosa clearly seen
- `3` — 3 – Entire mucosa clearly seen

## Method edition

BBPS/Lai 2009: 3 segments 0–3 after washing/suction; total 0–9

## Documented formula

Each segment scores 0 to 3 after washing and suction:

0: unprepared segment; mucosa obscured by solid stool that cannot be cleared.

1: some mucosa visible; other areas obscured by staining, residual stool or opaque liquid.

2: minor residue; mucosa well seen.

3: all mucosa well seen, no residue.

Total 0 to 9.

## Limits and population

BBPS was developed to score cleanliness observed during inspection after washing and suction by the endoscopist. The original single-center study does not automatically confirm adequacy cutoffs or repeat intervals adopted in later recommendations. Assessment of each segment and the edition of those criteria must be preserved.

## References

- [Lai EJ et al. The Boston bowel preparation scale: a valid and reliable instrument for colonoscopy-oriented research. Gastrointest Endosc, 2009.](https://doi.org/10.1016/j.gie.2008.05.057)

- [Calderwood AH, Jacobson BC. Comprehensive validation of the Boston Bowel Preparation Scale. Gastrointest Endosc, 2010.](https://doi.org/10.1016/j.gie.2010.06.068)

- [Johnson DA et al. Optimizing adequacy of bowel cleansing for colonoscopy: recommendations from the US Multi-Society Task Force on Colorectal Cancer. Gastroenterology, 2014.](https://doi.org/10.1053/j.gastro.2014.07.002)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
