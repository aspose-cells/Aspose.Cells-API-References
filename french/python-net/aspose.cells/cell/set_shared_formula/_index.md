---
title: set_shared_formula méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 330
url: /fr/python-net/aspose.cells/cell/set_shared_formula/
is_root: false
---
##  set_shared_formula(shared_formula, row_number, column_number) {#str-int-int}
Définit les formules partagées sur une plage de cellules.



```python
def set_shared_formula(self, shared_formula, row_number, column_number):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| shared_formula | str | Formule partagée.|
| row_number | int | Nombre de lignes pour remplir la formule.|
| column_number | int | Nombre de colonnes pour remplir la formule.|
###  Remarques



##  set_shared_formula(shared_formula, row_number, column_number, options) {#str-int-int-FormulaParseOptions}

Définit les formules partagées sur une plage de cellules.



```python
def set_shared_formula(self, shared_formula, row_number, column_number, options):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| shared_formula | str | Formule partagée.|
| row_number | int | Nombre de lignes pour remplir la formule.|
| column_number | int | Nombre de colonnes pour remplir la formule.|
| options | [FormulaParseOptions](/cells/fr/python-net/aspose.cells/formulaparseoptions) | Options d'analyse de la formule.|


##  set_shared_formula(shared_formula, row_number, column_number, is_r1c1, is_local) {#str-int-int-bool-bool}
Définit une formule sur une plage de cellules.



```python
def set_shared_formula(self, shared_formula, row_number, column_number, is_r1c1, is_local):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| shared_formula | str | Formule partagée.|
| row_number | int | Nombre de lignes pour remplir la formule.|
| column_number | int | Nombre de colonnes pour remplir la formule.|
| is_r1c1 | bool | si la formule est la formule R1C1|
| is_local | bool | si la formule est au format local|
###  Remarques

REMARQUE : Cette classe est désormais obsolète. Plutôt,
veuillez utiliser Cell.SetSharedFormula(string,int,int,FormulaParseOptions).
Cette propriété sera supprimée 12 mois plus tard depuis décembre 2019.
Aspose s'excuse pour tout inconvénient que vous pourriez avoir rencontré.

##  set_shared_formula(shared_formula, row_number, column_number, options, values) {#str-int-int-FormulaParseOptions-list}
Définit les formules partagées sur une plage de cellules.



```python
def set_shared_formula(self, shared_formula, row_number, column_number, options, values):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| shared_formula | str | Formule partagée.|
| row_number | int | Nombre de lignes pour remplir la formule.|
| column_number | int | Nombre de colonnes pour remplir la formule.|
| options | [FormulaParseOptions](/cells/fr/python-net/aspose.cells/formulaparseoptions) | Options d'analyse de la formule.|
| values | list | valeurs pour les cellules avec une formule partagée donnée|



###  Voir également
* module [aspose.cells](../../)
* classe [Cell](/cells/fr/python-net/aspose.cells/cell)
