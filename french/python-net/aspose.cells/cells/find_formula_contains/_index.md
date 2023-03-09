---
title: find_formula_contains méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 310
url: /fr/python-net/aspose.cells/cells/find_formula_contains/
is_root: false
---
##  find_formula_contains(formula, previous_cell) {#str-Cell}
Recherche la cellule avec la formule qui contient la chaîne d'entrée.


###  Retour

Cell objet.


```python
def find_formula_contains(self, formula, previous_cell):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| formula | str | La formule à rechercher.|
| previous_cell | [Cell](/cells/fr/python-net/aspose.cells/cell) |Cellule précédente avec la même formule. Ce paramètre peut être défini sur null si la recherche commence depuis le début.|
###  Remarques

Renvoie null (Nothing) si aucune cellule n'est trouvée.
 REMARQUE : ce membre est désormais obsolète.
veuillez utiliser la méthode Cells.Find(object,Cell,FindOptions) avec LookInType comme LookInType.OnlyFormulas
 et LookAtType comme LookAtType.Contains.
 Ce membre sera supprimé 12 mois plus tard depuis novembre 2018.
Aspose s'excuse pour tout inconvénient que vous pourriez avoir rencontré.


###  Voir également
* module [aspose.cells](../../)
* classe [Cells](/cells/fr/python-net/aspose.cells/cells)
