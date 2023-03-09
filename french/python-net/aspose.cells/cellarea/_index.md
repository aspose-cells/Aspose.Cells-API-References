---
title: CellArea classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 150
url: /fr/python-net/aspose.cells/cellarea/
is_root: false
---
##  CellArea classe
Représente une zone de cellules.



Le type CellArea expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [CellArea()](/cells/fr/python-net/aspose.cells/cellarea/__init__/#) | Construit une nouvelle instance de CellArea|


###  Propriétés
| Propriété| Description|
| :- | :- |
| [start_row](/cells/fr/python-net/aspose.cells/cellarea/start_row) | Obtient ou définit la ligne de début de cette zone.|
| [end_row](/cells/fr/python-net/aspose.cells/cellarea/end_row) | Obtient ou définit la ligne de fin de cette zone.|
| [start_column](/cells/fr/python-net/aspose.cells/cellarea/start_column) | Obtient ou définit la colonne de début de cette zone.|
| [end_column](/cells/fr/python-net/aspose.cells/cellarea/end_column) | Obtient ou définit la colonne de fin de cette zone.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [create_cell_area(start_row, start_column, end_row, end_column)](/cells/fr/python-net/aspose.cells/cellarea/create_cell_area/#int-int-int-int) | Crée une zone de cellule.|
| [create_cell_area(start_cell_name, end_cell_name)](/cells/fr/python-net/aspose.cells/cellarea/create_cell_area/#str-str) | Crée une zone de cellule.|
| [compare_to(obj)](/cells/fr/python-net/aspose.cells/cellarea/compare_to/#any) | Comparez deux objets CellArea en fonction de leur coin supérieur gauche.|



###  Exemple

```python
from aspose.cells import CellArea

# Create Cell Area
ca = CellArea()
ca.start_row = 0
ca.end_row = 0
ca.start_column = 0
ca.end_column = 0

```

###  Voir également
* module [aspose.cells](..)
