<!-- ELUCENIA technical documentation · volume-prostatico · es · no clinical/professional/rights approval -->

# Volumen prostático (elipsoide)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/volume-prostatico)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Diámetro longitudinal (craneocaudal)

`long`

cm · intervalo: 1–15

### Diámetro transversal (laterolateral)

`transv`

cm · intervalo: 1–15

### Diámetro anteroposterior

`ap`

cm · intervalo: 1–15

### PSA total (opcional, para la densidad)

`psa`

ng/mL · opcional · intervalo: 0,1–1000

## Edición del método

Elipsoide π/6×3 diámetros/Terris–Stamey 1991; densidad PSA=PSA/volumen

## Fórmula documentada

Volumen (mL) = π/6 × longitudinal × transverso × anteroposterior (cm), aproximadamente 0,52 × producto de tres medidas.

Densidad PSA = PSA ÷ Volumen.

## Límites y población

La fórmula elipsoide es una aproximación geométrica. El estudio citado comparó estimaciones por ecografía transrectal con el peso de piezas quirúrgicas y observó diferencias de rendimiento entre métodos y tamaños. No confirma automáticamente equivalencia entre RM y ecografía ni un diagnóstico por densidad de PSA.

## Referencias

- [Terris MK, Stamey TA. Determination of prostate volume by transrectal ultrasound. J Urol, 1991.](https://doi.org/10.1016/S0022-5347(17)38508-7)

- [Lerner LB et al. Management of lower urinary tract symptoms attributed to benign prostatic hyperplasia: AUA guideline part I, initial work-up and medical management. J Urol, 2021.](https://doi.org/10.1097/JU.0000000000002183)

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

## Resultados documentados

La información siguiente conserva las salidas del método para ejemplos sintéticos. No constituye una validación clínica independiente.

### 1

Próstata aumentada (30 a 80 mL)

| Detalles del resultado | |
| --- | --- |
| Fórmula del elipsoide (π/6 ≈ 0,52) | 4,0 × 4,5 × 3,5 cm |


### 2

Próstata aumentada (30 a 80 mL)

| Detalles del resultado | |
| --- | --- |
| Fórmula del elipsoide (π/6 ≈ 0,52) | 5,0 × 6,0 × 5,0 cm |
| Densidad del PSA | 0,05 ng/mL/cm³ |


### 3

Próstata muy aumentada (> 80 mL)

| Detalles del resultado | |
| --- | --- |
| Fórmula del elipsoide (π/6 ≈ 0,52) | 6,0 × 7,0 × 6,0 cm |

