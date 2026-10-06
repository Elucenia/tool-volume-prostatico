<!-- ELUCENIA technical documentation · volume-prostatico · pt-BR · no clinical/professional/rights approval -->

# Volume prostático (elipsoide)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/volume-prostatico)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Diâmetro longitudinal (craniocaudal)

`long`

cm · intervalo: 1–15

### Diâmetro transverso (laterolateral)

`transv`

cm · intervalo: 1–15

### Diâmetro anteroposterior

`ap`

cm · intervalo: 1–15

### PSA total (opcional, para a densidade)

`psa`

ng/mL · opcional · intervalo: 0,1–1000

## Edição do método

Elipsoideπ/6×3 diâmetros/Terris Stamey 1991; PSAdensidade PSA/volume

## Fórmula documentada

Volume (mL) = π/6 × longitudinal × transverso × anteroposterior (cm), ou seja, cerca de 0,52 × produto das três medidas.

Densidade do PSA = PSA ÷ volume.

## Limites e população

A fórmula elipsoide é uma aproximação geométrica. O estudo citado comparou estimativas por ultrassom transretal ao peso de peças cirúrgicas e observou desempenho diferente entre métodos e tamanhos. Não confirma automaticamente equivalência entre RM e ultrassom ou diagnóstico por densidade de PSA.

## Referências

- [Terris MK, Stamey TA. Determination of prostate volume by transrectal ultrasound. J Urol, 1991.](https://doi.org/10.1016/S0022-5347(17)38508-7)

- [Lerner LB et al. Management of lower urinary tract symptoms attributed to benign prostatic hyperplasia: AUA guideline part I, initial work-up and medical management. J Urol, 2021.](https://doi.org/10.1097/JU.0000000000002183)

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

Próstata aumentada (30 a 80 mL)

| Detalhes do resultado | |
| --- | --- |
| Fórmula do elipsoide (π/6 ≈ 0,52) | 4,0 × 4,5 × 3,5 cm |


### 2

Próstata aumentada (30 a 80 mL)

| Detalhes do resultado | |
| --- | --- |
| Fórmula do elipsoide (π/6 ≈ 0,52) | 5,0 × 6,0 × 5,0 cm |
| Densidade do PSA | 0,05 ng/mL/cm³ |


### 3

Próstata muito aumentada (> 80 mL)

| Detalhes do resultado | |
| --- | --- |
| Fórmula do elipsoide (π/6 ≈ 0,52) | 6,0 × 7,0 × 6,0 cm |

