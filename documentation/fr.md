<!-- ELUCENIA technical documentation · volume-prostatico · fr · no clinical/professional/rights approval -->

# Volume prostatique (ellipsoïde)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/volume-prostatico)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Diamètre longitudinal (crânio-caudal)

`long`

cm · intervalle: 1–15

### Diamètre transversal (latéro-latéral)

`transv`

cm · intervalle: 1–15

### Diamètre antéropostérieur

`ap`

cm · intervalle: 1–15

### PSA total (facultatif, pour la densité)

`psa`

ng/mL · facultatif · intervalle: 0,1–1000

## Édition de la méthode

Ellipsoïde π/6×3 diamètres/Terris–Stamey 1991; densité PSA=PSA/volume

## Formule documentée

Volume (mL) = π/6 × longitudinal × transverse × antéropostérieur (cm), environ 0,52 × produit des trois mesures.

Densité PSA = PSA ÷ Volume.

## Limites et population

La formule ellipsoïdale est une approximation géométrique. L’étude citée a comparé les estimations par échographie transrectale au poids des pièces opératoires et observé des performances différentes selon les méthodes et les tailles. Elle ne confirme pas automatiquement une équivalence entre IRM et échographie ou un diagnostic par la densité du PSA.

## Références

- [Terris MK, Stamey TA. Determination of prostate volume by transrectal ultrasound. J Urol, 1991.](https://doi.org/10.1016/S0022-5347(17)38508-7)

- [Lerner LB et al. Management of lower urinary tract symptoms attributed to benign prostatic hyperplasia: AUA guideline part I, initial work-up and medical management. J Urol, 2021.](https://doi.org/10.1097/JU.0000000000002183)

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
