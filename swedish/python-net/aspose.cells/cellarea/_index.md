---
title: CellArea klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 150
url: /sv/python-net/aspose.cells/cellarea/
is_root: false
---
##  CellArea klass
Representerar ett område av celler.



Typen CellArea avslöjar följande medlemmar:

###  Konstruktörer
| Konstruktör| Beskrivning|
| :- | :- |
| [CellArea()](/cells/sv/python-net/aspose.cells/cellarea/__init__/#) | Konstruerar en ny instans av CellArea|


###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [start_row](/cells/sv/python-net/aspose.cells/cellarea/start_row) | Hämtar eller ställer in startraden för detta område.|
| [end_row](/cells/sv/python-net/aspose.cells/cellarea/end_row) | Hämtar eller ställer in den sista raden för detta område.|
| [start_column](/cells/sv/python-net/aspose.cells/cellarea/start_column) |Hämtar eller ställer in startkolumnen för detta område.|
| [end_column](/cells/sv/python-net/aspose.cells/cellarea/end_column) | Hämtar eller ställer in slutkolumnen för detta område.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [create_cell_area(start_row, start_column, end_row, end_column)](/cells/sv/python-net/aspose.cells/cellarea/create_cell_area/#int-int-int-int) | Skapar ett cellområde.|
| [create_cell_area(start_cell_name, end_cell_name)](/cells/sv/python-net/aspose.cells/cellarea/create_cell_area/#str-str) | Skapar ett cellområde.|
| [compare_to(obj)](/cells/sv/python-net/aspose.cells/cellarea/compare_to/#any) | Jämför två CellArea-objekt enligt deras övre vänstra hörn.|



###  Exempel

```python
from aspose.cells import CellArea

# Create Cell Area
ca = CellArea()
ca.start_row = 0
ca.end_row = 0
ca.start_column = 0
ca.end_column = 0

```

###  Se även
* modul [aspose.cells](..)
