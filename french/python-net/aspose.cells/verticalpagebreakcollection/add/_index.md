---
title: add méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 20
url: /fr/python-net/aspose.cells/verticalpagebreakcollection/add/
is_root: false
---
##  add(column) {#int}
Ajoute un saut de page vertical à la collection.


###  Retour

[VerticalPageBreak](/cells/fr/python-net/aspose.cells/verticalpagebreak) indice d'objet.


```python
def add(self, column):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| column | int | Cell index de colonne, basé sur zéro.|
###  Remarques

Un saut de page est ajouté en haut à gauche de la cellule.
Veuillez définir simultanément un saut de page horizontal et un saut de page vertical.

##  add(cell_name) {#str}
Ajoute un saut de page vertical à la collection.


###  Retour

[VerticalPageBreak](/cells/fr/python-net/aspose.cells/verticalpagebreak) indice d'objet.


```python
def add(self, cell_name):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| cell_name | str | Cell nom.|
###  Remarques

Un saut de page est ajouté en haut à gauche de la cellule.
Veuillez définir simultanément un saut de page horizontal et un saut de page vertical.

##  add(row, column) {#int-int}
Ajoute un saut de page vertical à la collection.


###  Retour

[VerticalPageBreak](/cells/fr/python-net/aspose.cells/verticalpagebreak) indice d'objet.


```python
def add(self, row, column):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| row | int | Cell index de ligne, basé sur zéro.|
| column | int | Cell index de colonne, basé sur zéro.|
###  Remarques

Un saut de page est ajouté en haut à gauche de la cellule.
Veuillez définir simultanément un saut de page horizontal et un saut de page vertical.

##  add(start_row, end_row, column) {#int-int-int}
Ajoute un saut de page vertical à la collection.


###  Retour

[VerticalPageBreak](/cells/fr/python-net/aspose.cells/verticalpagebreak) indice d'objet.


```python
def add(self, start_row, end_row, column):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| start_row | int | Index de ligne de début, basé sur zéro.|
| end_row | int |Index de fin de ligne, basé sur zéro.|
| column | int | Index de colonne, basé sur zéro.|
###  Remarques

Cette méthode est utilisée pour add un saut de page vertical dans une zone d'impression.


###  Voir également

* module [aspose.cells](../../)
* classe [VerticalPageBreak](/cells/fr/python-net/aspose.cells/verticalpagebreak)
* classe [VerticalPageBreakCollection](/cells/fr/python-net/aspose.cells/verticalpagebreakcollection)
