---
title: change_palette méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 50
url: /fr/python-net/aspose.cells/workbook/change_palette/
is_root: false
---
##  change_palette(color, index) {#aspose.pydrawing.Color-int}
Modifie la palette de la feuille de calcul dans l'index spécifié.



```python
def change_palette(self, color, index):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| color | aspose.pydrawing.Color | Structure de couleur.|
| index | int | Indice de palette, 0 - 55.|
###  Remarques

La palette comporte 56 entrées, chacune représentée par une valeur RVB.


Si vous définissez une couleur qui n'est pas dans la palette, elle ne prendra pas effet.


Donc, si vous souhaitez définir une couleur personnalisée, veuillez d'abord modifier la palette.


Voici la palette de couleurs standard.

| Couleur| Rouge| Vert| Bleu|
| :- | :- | :- | :- |
| Noir| 0| 0| 0 |
| Blanc| 255| 255| 255 |
| Rouge| 255| 0| 0 |
| Chaux| 0| 255| 0 |
| Bleu| 0| 0| 255 |
| Jaune| 255| 255| 0 |
| Magenta| 255| 0| 255 |
| cyan| 0| 255| 255 |
| Bordeaux| 128| 0| 0 |
| Vert| 0| 128| 0 |
| Marine| 0| 0| 128 |
| olive| 128| 128| 0 |
| Violet| 128| 0| 128 |
| Sarcelle| 0| 128| 128 |
| Argent| 192| 192| 192 |
| Gris| 128| 128| 128 |
| Couleur17| 153| 153| 255 |
| Couleur18| 153| 51| 102 |
| Couleur19| 255| 255| 204 |
| Couleur20| 204| 255| 255 |
| Couleur21| 102| 0| 102 |
| Couleur22| 255| 128| 128 |
| Couleur23| 0| 102| 204 |
| Couleur24| 204| 204| 255 |
| Couleur25| 0| 0| 128 |
| Couleur26| 255| 0| 255 |
| Couleur27| 255| 255| 0 |
| Couleur28| 0| 255| 255 |
| Couleur29| 128| 0| 128 |
| Couleur30| 128| 0| 0 |
| Couleur31| 0| 128| 128 |
| Couleur32| 0| 0| 255 |
| Couleur33| 0| 204| 255 |
| Couleur34| 204| 255| 255 |
| Couleur35| 204| 255| 204 |
| Couleur36| 255| 255| 153 |
| Couleur37| 153| 204| 255 |
| Couleur38| 255| 153| 204 |
| Couleur39| 204| 153| 255 |
| Couleur40| 255| 204| 153 |
| Couleur41| 51| 102| 255 |
| Couleur42| 51| 204| 204 |
| Couleur43| 153| 204| 0 |
| Couleur44| 255| 204| 0 |
| Couleur45| 255| 153| 0 |
| Couleur46| 255| 102| 0 |
| Couleur47| 102| 102| 153 |
| Couleur48| 150| 150| 150 |
| Couleur49| 0| 51| 102 |
| Couleur50| 51| 153| 102 |
| Couleur51| 0| 51| 0 |
| Couleur52| 51| 51| 0 |
| Couleur53| 153| 51| 0 |
|Couleur54| 153| 51| 102 |
| Couleur55| 51| 51| 153 |
| Couleur56| 51| 51| 51 |


###  Voir également

* module [aspose.cells](../../)
* classe [Workbook](/cells/fr/python-net/aspose.cells/workbook)
