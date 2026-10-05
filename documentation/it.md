<!-- ELUCENIA technical documentation · volume-prostatico · it · no clinical/professional/rights approval -->

# Volume prostatico (ellissoide)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/volume-prostatico)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Diametro longitudinale (craniocaudale)

`long`

cm · intervallo: 1–15

### Diametro trasverso (laterolaterale)

`transv`

cm · intervallo: 1–15

### Diametro anteroposteriore

`ap`

cm · intervallo: 1–15

### PSA totale (facoltativo, per la densità)

`psa`

ng/mL · facoltativo · intervallo: 0,1–1000

## Edizione del metodo

Ellissoide π/6×3 diametri/Terris–Stamey 1991; densità PSA=PSA/volume

## Formula documentata

Volume (mL) = π/6 × longitudinale × trasverso × anteroposteriore (cm), circa 0,52 × prodotto di tre misure.

Densità PSA = PSA ÷ Volume.

## Limiti e popolazione

La formula dell’ellissoide è un’approssimazione geometrica. Lo studio citato ha confrontato le stime mediante ecografia transrettale con il peso dei pezzi chirurgici e ha osservato prestazioni diverse tra metodi e dimensioni. Non conferma automaticamente l’equivalenza tra RM ed ecografia o una diagnosi mediante densità del PSA.

## Riferimenti

- [Terris MK, Stamey TA. Determination of prostate volume by transrectal ultrasound. J Urol, 1991.](https://doi.org/10.1016/S0022-5347(17)38508-7)

- [Lerner LB et al. Management of lower urinary tract symptoms attributed to benign prostatic hyperplasia: AUA guideline part I, initial work-up and medical management. J Urol, 2021.](https://doi.org/10.1097/JU.0000000000002183)

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
