---
title: start_cell méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 40
url: /fr/python-net/aspose.cells/lightcellsdatahandler/start_cell/
is_root: false
---
##  start_cell(column_index) {#int}
Se prépare à traiter une cellule.


###  Retour

si cette cellule doit être traitée. false pour ignorer la cellule et vérifier la suivante jusqu'à atteindre la fin des données des cellules de la ligne actuelle


```python
def start_cell(self, column_index):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| column_index | int | index de colonne de la cellule à traiter|
###  Remarques

Il sera appelé lorsqu'il atteindra une cellule existante dans la ligne actuelle. La ligne actuelle est la ligne du dernier appel du [LightCellsDataHandler.process_row(row)](/cells/fr/python-net/aspose.cells/lightcellsdatahandler/process_row).


###  Voir également

* module [aspose.cells](../../)
* classe [LightCellsDataHandler](/cells/fr/python-net/aspose.cells/lightcellsdatahandler)
