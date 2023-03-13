---
title: set_array_formula méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 290
url: /fr/python-net/aspose.cells/cell/set_array_formula/
is_root: false
---
##  set_array_formula(array_formula, row_number, column_number) {#str-int-int}
Définit une formule matricielle (formule matricielle héritée saisie via CTRL + MAJ + ENTRÉE dans ms excel) sur une plage de cellules.



```python
def set_array_formula(self, array_formula, row_number, column_number):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| array_formula | str | Formule matricielle.|
| row_number | int |Nombre de lignes pour remplir le résultat de la formule matricielle.|
| column_number | int | Nombre de colonnes pour remplir le résultat de la formule matricielle.|


##  set_array_formula(array_formula, row_number, column_number, options) {#str-int-int-FormulaParseOptions}
Définit une formule matricielle sur une plage de cellules.



```python
def set_array_formula(self, array_formula, row_number, column_number, options):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| array_formula | str | Formule matricielle.|
| row_number | int |Nombre de lignes pour remplir le résultat de la formule matricielle.|
| column_number | int | Nombre de colonnes pour remplir le résultat de la formule matricielle.|
| options | [FormulaParseOptions](/cells/fr/python-net/aspose.cells/formulaparseoptions) | Options d'analyse de la formule.|


##  set_array_formula(array_formula, row_number, column_number, is_r1c1, is_local) {#str-int-int-bool-bool}
Définit une formule matricielle sur une plage de cellules.



```python
def set_array_formula(self, array_formula, row_number, column_number, is_r1c1, is_local):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| array_formula | str | Formule matricielle.|
| row_number | int |Nombre de lignes pour remplir le résultat de la formule matricielle.|
| column_number | int | Nombre de colonnes pour remplir le résultat de la formule matricielle.|
| is_r1c1 | bool | si la formule est la formule R1C1|
| is_local | bool | si la formule est au format local|
###  Remarques

REMARQUE : Cette classe est désormais obsolète. Plutôt,
veuillez utiliser Cell.SetArrayFormula(string,int,int,FormulaParseOptions).
Cette propriété sera supprimée 12 mois plus tard depuis décembre 2019.
Aspose s'excuse pour tout inconvénient que vous pourriez avoir rencontré.

##  set_array_formula(array_formula, row_number, column_number, options, values) {#str-int-int-FormulaParseOptions-list}
Définit une formule matricielle sur une plage de cellules.



```python
def set_array_formula(self, array_formula, row_number, column_number, options, values):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| array_formula | str | Formule matricielle.|
| row_number | int |Nombre de lignes pour remplir le résultat de la formule matricielle.|
| column_number | int | Nombre de colonnes pour remplir le résultat de la formule matricielle.|
| options | [FormulaParseOptions](/cells/fr/python-net/aspose.cells/formulaparseoptions) | Options d'analyse de la formule.|
| values | list | valeurs pour ces cellules avec une formule matricielle donnée|



###  Voir également
* module [aspose.cells](../../)
* classe [Cell](/cells/fr/python-net/aspose.cells/cell)
