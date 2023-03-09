---
title: process_row méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 30
url: /fr/python-net/aspose.cells/lightcellsdatahandler/process_row/
is_root: false
---
##  process_row(row) {#Row}
Commence à traiter une ligne.


###  Retour

si les cellules de cette ligne doivent être traitées. false pour ignorer toutes les cellules de cette ligne.


```python
def process_row(self, row):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| row | [Row](/cells/fr/python-net/aspose.cells/row) | Objet de ligne en cours de traitement.|
###  Remarques

Il sera appelé après les propriétés de la ligne telles que la hauteur, le style, etc. ont été lus. Cependant, les cellules de cette ligne n'ont pas encore été lues.


###  Voir également

* module [aspose.cells](../../)
* classe [LightCellsDataHandler](/cells/fr/python-net/aspose.cells/lightcellsdatahandler)
