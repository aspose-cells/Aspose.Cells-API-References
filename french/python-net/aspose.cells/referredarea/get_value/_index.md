---
title: get_value méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 20
url: /fr/python-net/aspose.cells/referredarea/get_value/
is_root: false
---
##  get_value(row_offset, col_offset) {#int-int}
Obtient la valeur de la cellule avec un décalage donné à partir du coin supérieur gauche de cette zone.


###  Retour

"#REF !" si cette zone est invalide ;
"#N/A" s'il est donné un décalage hors de cette zone ;
Sinon, renvoie la valeur de la cellule à la position donnée.


```python
def get_value(self, row_offset, col_offset):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| row_offset | int | décalage de ligne par rapport à la ligne de départ de cette zone|
| col_offset | int | décalage de colonne par rapport à la ligne de départ de cette zone|


##  get_value(row_offset, col_offset, calculate_formulas) {#int-int-bool}
Obtient la valeur de la cellule avec un décalage donné à partir du coin supérieur gauche de cette zone.


###  Retour

"#REF !" si cette zone est invalide ;
"#N/A" s'il est donné un décalage hors de cette zone ;
Sinon, renvoie la valeur de la cellule à la position donnée.


```python
def get_value(self, row_offset, col_offset, calculate_formulas):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| row_offset | int | décalage de ligne par rapport à la ligne de départ de cette zone|
| col_offset | int | décalage de colonne par rapport à la ligne de départ de cette zone|
| calculate_formulas | bool | Que ce soit pour le calculer récursivement si la référence spécifiée est une formule|



###  Voir également
* module [aspose.cells](../../)
* classe [ReferredArea](/cells/fr/python-net/aspose.cells/referredarea)
