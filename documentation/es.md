<!-- ELUCENIA technical documentation · boston-bowel-preparation-scale · es · no clinical/professional/rights approval -->

# Escala de preparación intestinal de Boston (BBPS)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/boston-bowel-preparation-scale)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Colon derecho (ciego y ascendente)

`dir`

- `0` — 0 – Mucosa no visible (heces sólidas)
- `1` — 1 – Parte de la mucosa visible
- `2` — 2 – Residuo mínimo, mucosa bien visible
- `3` — 3 – Toda la mucosa bien visible

### Colon transverso (incluidas las flexuras)

`trans`

- `0` — 0 – Mucosa no visible (heces sólidas)
- `1` — 1 – Parte de la mucosa visible
- `2` — 2 – Residuo mínimo, mucosa bien visible
- `3` — 3 – Toda la mucosa bien visible

### Colon izquierdo (descendente, sigmoide y recto)

`esq`

- `0` — 0 – Mucosa no visible (heces sólidas)
- `1` — 1 – Parte de la mucosa visible
- `2` — 2 – Residuo mínimo, mucosa bien visible
- `3` — 3 – Toda la mucosa bien visible

## Edición del método

BBPS/Lai 2009: 3 segmentos 0–3 tras lavado/aspiración; total 0–9

## Fórmula documentada

Cada segmento recibe 0 a 3 después de lavado y aspiración:

0: sin preparar; mucosa oculta por heces sólidas que no se eliminan.

1: parte visible; otras zonas cubiertas por manchas, heces residuales o líquido opaco.

2: pocos residuos, mucosa bien visible.

3: toda la mucosa visible, sin residuos.

Total 0 a 9.

## Límites y población

La BBPS se desarrolló para puntuar la limpieza observada durante la inspección tras el lavado y la aspiración por el endoscopista. El estudio original de un solo centro no confirma automáticamente los puntos de corte de adecuación ni los intervalos de repetición adoptados en recomendaciones posteriores. Deben conservarse la evaluación de cada segmento y la edición de esos criterios.

## Referencias

- [Lai EJ et al. The Boston bowel preparation scale: a valid and reliable instrument for colonoscopy-oriented research. Gastrointest Endosc, 2009.](https://doi.org/10.1016/j.gie.2008.05.057)

- [Calderwood AH, Jacobson BC. Comprehensive validation of the Boston Bowel Preparation Scale. Gastrointest Endosc, 2010.](https://doi.org/10.1016/j.gie.2010.06.068)

- [Johnson DA et al. Optimizing adequacy of bowel cleansing for colonoscopy: recommendations from the US Multi-Society Task Force on Colorectal Cancer. Gastroenterology, 2014.](https://doi.org/10.1053/j.gastro.2014.07.002)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
