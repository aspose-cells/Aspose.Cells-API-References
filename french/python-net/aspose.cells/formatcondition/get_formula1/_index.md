---
title: get_formula1 méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 20
url: /fr/python-net/aspose.cells/formatcondition/get_formula1/
is_root: false
---
##  get_formula1(is_r1c1, is_local) {#bool-bool}
Obtient la valeur ou l'expression associée à cette condition de format.


###  Retour

La valeur ou l'expression associée à cette condition de format.


```python
def get_formula1(self, is_r1c1, is_local):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| is_r1c1 | bool | Indique si la formule doit être formatée en tant que R1C1.|
| is_local | bool | Indique si la formule doit être formatée par les paramètres régionaux.|


##  get_formula1(row, column) {#int-int}
Obtient la formule de la mise en forme conditionnelle de la cellule.


###  Retour

La formule.


```python
def get_formula1(self, row, column):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| row | int | L'index de ligne.|
| column | int | L'indice de colonne.|


##  get_formula1(is_r1c1, is_local, row, column) {#bool-bool-int-int}
Obtient la valeur ou l'expression de la mise en forme conditionnelle de la cellule.


###  Retour

La valeur ou l'expression associée à la mise en forme conditionnelle de la cellule.


```python
def get_formula1(self, is_r1c1, is_local, row, column):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| is_r1c1 | bool | Indique si la formule doit être formatée en tant que R1C1.|
| is_local | bool | Indique si la formule doit être formatée par les paramètres régionaux.|
| row | int | L'index de ligne.|
| column | int | L'indice de colonne.|
###  Remarques

La cellule donnée doit être contenue par cette mise en forme conditionnelle, sinon null sera renvoyé.


###  Voir également

* module [aspose.cells](../../)
* classe [FormatCondition](/cells/fr/python-net/aspose.cells/formatcondition)
