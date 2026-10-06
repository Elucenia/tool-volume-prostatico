<!-- ELUCENIA technical documentation · volume-prostatico · de · no clinical/professional/rights approval -->

# Prostatavolumen (Ellipsoid)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/volume-prostatico)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Längsdurchmesser (kraniokaudal)

`long`

cm · Bereich: 1–15

### Querdurchmesser (laterolateral)

`transv`

cm · Bereich: 1–15

### Anteroposteriorer Durchmesser

`ap`

cm · Bereich: 1–15

### Gesamt-PSA (optional, für die Dichte)

`psa`

ng/mL · optional · Bereich: 0,1–1000

## Fassung der Methode

Ellipsoid π/6×3 Durchmesser/Terris–Stamey 1991; PSA-Dichte=PSA/Volumen

## Dokumentierte Formel

Volumen (mL) = π/6 × längs × quer × anteroposterior (cm), etwa 0,52 × Produkt der drei Maße.

PSA-Dichte = PSA ÷ Volumen.

## Grenzen und Population

Die Ellipsoidformel ist eine geometrische Näherung. Die zitierte Studie verglich transrektale Ultraschallschätzungen mit dem Gewicht von Operationspräparaten und fand unterschiedliche Leistung je Methode und Größe. Sie bestätigt nicht automatisch eine Gleichwertigkeit von MRT und Ultraschall oder eine Diagnose anhand der PSA-Dichte.

## Referenzen

- [Terris MK, Stamey TA. Determination of prostate volume by transrectal ultrasound. J Urol, 1991.](https://doi.org/10.1016/S0022-5347(17)38508-7)

- [Lerner LB et al. Management of lower urinary tract symptoms attributed to benign prostatic hyperplasia: AUA guideline part I, initial work-up and medical management. J Urol, 2021.](https://doi.org/10.1097/JU.0000000000002183)

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

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

Vergrößerte Prostata (30 bis 80 mL)

| Ergebnisdetails | |
| --- | --- |
| Ellipsoidformel (π/6 ≈ 0,52) | 4,0 × 4,5 × 3,5 cm |


### 2

Vergrößerte Prostata (30 bis 80 mL)

| Ergebnisdetails | |
| --- | --- |
| Ellipsoidformel (π/6 ≈ 0,52) | 5,0 × 6,0 × 5,0 cm |
| PSA-Dichte | 0,05 ng/mL/cm³ |


### 3

Deutlich vergrößerte Prostata (> 80 mL)

| Ergebnisdetails | |
| --- | --- |
| Ellipsoidformel (π/6 ≈ 0,52) | 6,0 × 7,0 × 6,0 cm |

