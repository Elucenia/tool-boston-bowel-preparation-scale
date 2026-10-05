<!-- ELUCENIA technical documentation · boston-bowel-preparation-scale · de · no clinical/professional/rights approval -->

# Boston-Skala zur Darmvorbereitung (BBPS)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/boston-bowel-preparation-scale)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Rechter Dickdarm (Zökum und Colon ascendens)

`dir`

- `0` — 0 – Schleimhaut nicht sichtbar (fester Stuhl)
- `1` — 1 – Ein Teil der Schleimhaut sichtbar
- `2` — 2 – Minimale Rückstände, Schleimhaut gut sichtbar
- `3` — 3 – Gesamte Schleimhaut gut sichtbar

### Querkolon (einschließlich Flexuren)

`trans`

- `0` — 0 – Schleimhaut nicht sichtbar (fester Stuhl)
- `1` — 1 – Ein Teil der Schleimhaut sichtbar
- `2` — 2 – Minimale Rückstände, Schleimhaut gut sichtbar
- `3` — 3 – Gesamte Schleimhaut gut sichtbar

### Linker Dickdarm (Colon descendens, Sigma und Rektum)

`esq`

- `0` — 0 – Schleimhaut nicht sichtbar (fester Stuhl)
- `1` — 1 – Ein Teil der Schleimhaut sichtbar
- `2` — 2 – Minimale Rückstände, Schleimhaut gut sichtbar
- `3` — 3 – Gesamte Schleimhaut gut sichtbar

## Fassung der Methode

BBPS/Lai 2009: 3 Segmente 0–3 nach Spülung/Absaugung; Gesamt 0–9

## Dokumentierte Formel

Jedes Segment erhält 0 bis 3 nach Spülung und Absaugung:

0: unvorbereitet; Schleimhaut durch nicht entfernbaren festen Stuhl verdeckt.

1: teilweise sichtbar; andere Bereiche durch Verfärbungen, Reststuhl oder trübe Flüssigkeit verdeckt.

2: geringe Reste, Schleimhaut gut sichtbar.

3: gesamte Schleimhaut gut sichtbar, keine Reste.

Gesamt 0 bis 9.

## Grenzen und Population

BBPS wurde zur Bewertung der bei der Inspektion nach Spülung und Absaugung durch den Endoskopierenden beobachteten Sauberkeit entwickelt. Die ursprüngliche Einzelzentrumsstudie bestätigt nicht automatisch später empfohlene Angemessenheitsschwellen oder Wiederholungsintervalle. Die Bewertung jedes Segments und die Ausgabe dieser Kriterien müssen erhalten bleiben.

## Referenzen

- [Lai EJ et al. The Boston bowel preparation scale: a valid and reliable instrument for colonoscopy-oriented research. Gastrointest Endosc, 2009.](https://doi.org/10.1016/j.gie.2008.05.057)

- [Calderwood AH, Jacobson BC. Comprehensive validation of the Boston Bowel Preparation Scale. Gastrointest Endosc, 2010.](https://doi.org/10.1016/j.gie.2010.06.068)

- [Johnson DA et al. Optimizing adequacy of bowel cleansing for colonoscopy: recommendations from the US Multi-Society Task Force on Colorectal Cancer. Gastroenterology, 2014.](https://doi.org/10.1053/j.gastro.2014.07.002)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026
