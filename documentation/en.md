<!-- ELUCENIA technical documentation · volume-prostatico · en · no clinical/professional/rights approval -->

# Prostate volume (ellipsoid)

[conditions, sources and permissions](https://elucenia.org/en/tools/volume-prostatico)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Longitudinal diameter (craniocaudal)

`long`

cm · range: 1–15

### Transverse diameter (laterolateral)

`transv`

cm · range: 1–15

### Anteroposterior diameter

`ap`

cm · range: 1–15

### Total PSA (optional, for density)

`psa`

ng/mL · optional · range: 0.1–1000

## Method edition

Ellipsoid π/6×3 diameters/Terris–Stamey 1991; PSA density=PSA/volume

## Documented formula

Volume (mL) = π/6 × longitudinal × transverse × anteroposterior (cm), approximately 0.52 × product of three measurements.

PSA density = PSA ÷ Volume.

## Limits and population

The ellipsoid formula is a geometric approximation. The cited study compared transrectal ultrasound estimates with the weight of surgical specimens and found different performance across methods and sizes. It does not automatically confirm equivalence between MRI and ultrasound or diagnosis through PSA density.

## References

- [Terris MK, Stamey TA. Determination of prostate volume by transrectal ultrasound. J Urol, 1991.](https://doi.org/10.1016/S0022-5347(17)38508-7)

- [Lerner LB et al. Management of lower urinary tract symptoms attributed to benign prostatic hyperplasia: AUA guideline part I, initial work-up and medical management. J Urol, 2021.](https://doi.org/10.1097/JU.0000000000002183)

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
