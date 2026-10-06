<!-- ELUCENIA technical documentation · boston-bowel-preparation-scale · fr · no clinical/professional/rights approval -->

# Échelle de préparation colique de Boston (BBPS)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/boston-bowel-preparation-scale)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Côlon droit (cæcum et ascendant)

`dir`

- `0` — 0 – Muqueuse non visible (selles solides)
- `1` — 1 – Une partie de la muqueuse visible
- `2` — 2 – Résidus minimes, muqueuse bien visible
- `3` — 3 – Toute la muqueuse bien visible

### Côlon transverse (angles inclus)

`trans`

- `0` — 0 – Muqueuse non visible (selles solides)
- `1` — 1 – Une partie de la muqueuse visible
- `2` — 2 – Résidus minimes, muqueuse bien visible
- `3` — 3 – Toute la muqueuse bien visible

### Côlon gauche (descendant, sigmoïde et rectum)

`esq`

- `0` — 0 – Muqueuse non visible (selles solides)
- `1` — 1 – Une partie de la muqueuse visible
- `2` — 2 – Résidus minimes, muqueuse bien visible
- `3` — 3 – Toute la muqueuse bien visible

## Édition de la méthode

BBPS/Lai 2009 : 3 segments 0–3 après lavage/aspiration ; total 0–9

## Formule documentée

Chaque segment est coté 0 à 3 après lavage et aspiration :

0 : non préparé, muqueuse masquée par des selles solides non évacuables.

1 : une partie visible, d’autres zones masquées par coloration, selles résiduelles ou liquide opaque.

2 : peu de résidus, muqueuse bien visible.

3 : toute la muqueuse visible, sans résidus.

Total 0 à 9.

## Limites et population

La BBPS a été développée pour coter la propreté observée à l’inspection après lavage et aspiration par l’endoscopiste. L’étude monocentrique originale ne confirme pas automatiquement les seuils d’adéquation ou les intervalles de répétition adoptés par des recommandations ultérieures. L’évaluation de chaque segment et l’édition de ces critères doivent être conservées.

## Références

- [Lai EJ et al. The Boston bowel preparation scale: a valid and reliable instrument for colonoscopy-oriented research. Gastrointest Endosc, 2009.](https://doi.org/10.1016/j.gie.2008.05.057)

- [Calderwood AH, Jacobson BC. Comprehensive validation of the Boston Bowel Preparation Scale. Gastrointest Endosc, 2010.](https://doi.org/10.1016/j.gie.2010.06.068)

- [Johnson DA et al. Optimizing adequacy of bowel cleansing for colonoscopy: recommendations from the US Multi-Society Task Force on Colorectal Cancer. Gastroenterology, 2014.](https://doi.org/10.1053/j.gastro.2014.07.002)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

Préparation adéquate (total ≥ 6 et tous les segments ≥ 2)

| Détails du résultat | |
| --- | --- |
| Côlon droit | 3 |
| Côlon transverse | 3 |
| Côlon gauche | 3 |


### 2

Préparation adéquate (total ≥ 6 et tous les segments ≥ 2)

| Détails du résultat | |
| --- | --- |
| Côlon droit | 2 |
| Côlon transverse | 2 |
| Côlon gauche | 2 |


### 3

Préparation inadéquate : répéter la coloscopie à court intervalle

| Détails du résultat | |
| --- | --- |
| Côlon droit | 1 |
| Côlon transverse | 3 |
| Côlon gauche | 3 |

Total ≥ 6, mais il existe un segment avec un score < 2 : la préparation n’est pas considérée comme adéquate.


### 4

Préparation inadéquate : répéter la coloscopie à court intervalle

| Détails du résultat | |
| --- | --- |
| Côlon droit | 1 |
| Côlon transverse | 1 |
| Côlon gauche | 1 |

