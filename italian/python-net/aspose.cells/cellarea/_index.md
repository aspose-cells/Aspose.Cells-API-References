---
title: classe CellArea
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 150
url: /it/python-net/aspose.cells/cellarea/
is_root: false
---
##  classe CellArea
Rappresenta un'area di celle.



Il tipo CellArea espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [CellArea()](/cells/it/python-net/aspose.cells/cellarea/__init__/#) | Costruisce una nuova istanza di CellArea|


###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [start_row](/cells/it/python-net/aspose.cells/cellarea/start_row) | Ottiene o imposta la riga iniziale di quest'area.|
| [end_row](/cells/it/python-net/aspose.cells/cellarea/end_row) | Ottiene o imposta la riga finale di quest'area.|
| [start_column](/cells/it/python-net/aspose.cells/cellarea/start_column) | Ottiene o imposta la colonna iniziale di quest'area.|
| [end_column](/cells/it/python-net/aspose.cells/cellarea/end_column) | Ottiene o imposta la colonna finale di quest'area.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [create_cell_area(start_row, start_column, end_row, end_column)](/cells/it/python-net/aspose.cells/cellarea/create_cell_area/#int-int-int-int) | Crea un'area della cella.|
| [create_cell_area(start_cell_name, end_cell_name)](/cells/it/python-net/aspose.cells/cellarea/create_cell_area/#str-str) | Crea un'area della cella.|
| [compare_to(obj)](/cells/it/python-net/aspose.cells/cellarea/compare_to/#any) | Confronta due oggetti CellArea in base al loro angolo in alto a sinistra.|



###  Esempio

```python
from aspose.cells import CellArea

# Create Cell Area
ca = CellArea()
ca.start_row = 0
ca.end_row = 0
ca.start_column = 0
ca.end_column = 0

```

###  Guarda anche
* modulo [aspose.cells](..)
