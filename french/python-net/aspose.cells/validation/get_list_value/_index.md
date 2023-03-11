---
title: get_list_value méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 70
url: /fr/python-net/aspose.cells/validation/get_list_value/
is_root: false
---
##  get_list_value(row, column) {#int-int}
Obtenez la valeur de la liste de la validation pour la cellule spécifiée.


###  Retour

La valeur pour produire la liste de cette validation pour la cellule spécifiée.
Si la liste fait référence à une plage, la valeur renvoyée sera un objet [ReferredArea](/cells/fr/python-net/aspose.cells/referredarea) ;
Sinon, la valeur renvoyée peut être null, object[] ou simple object.


```python
def get_list_value(self, row, column):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| row | int | L'index de ligne.|
| column | int | L'indice de colonne.|
###  Remarques

Uniquement pour la validation dont le type est Liste et a été appliqué à une cellule donnée,
sinon null sera retourné.


###  Voir également
* module [aspose.cells](../../)
* classe [ReferredArea](/cells/fr/python-net/aspose.cells/referredarea)
* classe [Validation](/cells/fr/python-net/aspose.cells/validation)
