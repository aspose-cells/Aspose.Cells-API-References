---
title: get_dependents_in_calculation méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 390
url: /fr/python-net/aspose.cells/cells/get_dependents_in_calculation/
is_root: false
---
##  get_dependents_in_calculation(row, column, recursive) {#int-int-bool}
Obtient toutes les cellules dont le résultat calculé dépend d'une cellule spécifique.


###  Retour

Énumérateur pour énumérer toutes les personnes à charge (objets Cell)


```python
def get_dependents_in_calculation(self, row, column, recursive):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| row | int | Index de ligne de la cellule spécifique|
| column | int | Index de colonne de la cellule spécifique.|
| recursive | bool | Si renvoie les personnes à charge qui ne font pas directement référence à la cellule spécifique<br/> mais référence à d'autres feuilles de cette cellule.|
###  Remarques

Pour utiliser cette méthode, assurez-vous que le classeur a été défini avec la valeur true pour
[FormulaSettings.enable_calculation_chain](/cells/fr/python-net/aspose.cells/formulasettings#enable_calculation_chain) et a été entièrement calculé avec ce paramètre.
S'il n'y a pas de référence de formule à cette cellule, null sera renvoyé.
Pour plus de détails et d'exemples, veuillez consulter le [Cell.get_dependents_in_calculation(recursive)](/cells/fr/python-net/aspose.cells/cell/get_dependents_in_calculation)


###  Voir également
* module [aspose.cells](../../)
* classe [Cells](/cells/fr/python-net/aspose.cells/cells)
