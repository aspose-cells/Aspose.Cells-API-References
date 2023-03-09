---
title: ListColumn klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 10
url: /sv/python-net/aspose.cells.tables/listcolumn/
is_root: false
---
##  ListColumn klass
Representerar en kolumn i en lista.



Typen ListColumn avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [name](/cells/sv/python-net/aspose.cells.tables/listcolumn/name) | Hämtar och ställer in namnet på kolumnen.|
| [totals_calculation](/cells/sv/python-net/aspose.cells.tables/listcolumn/totals_calculation) | Hämtar och ställer in beräkningstypen i raden Totals i listkolumnen.|
| [range](/cells/sv/python-net/aspose.cells.tables/listcolumn/range) | Hämtar intervallet för den här listkolumnen.|
| [formula](/cells/sv/python-net/aspose.cells.tables/listcolumn/formula) | Hämtar och ställer in formeln för listkolumnen.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [get_custom_totals_row_formula(is_r1c1, is_local)](/cells/sv/python-net/aspose.cells.tables/listcolumn/get_custom_totals_row_formula/#bool-bool) | Hämtar formeln för totalraden i den här listkolumnen.|
| [set_custom_totals_row_formula(formula, is_r1c1, is_local)](/cells/sv/python-net/aspose.cells.tables/listcolumn/set_custom_totals_row_formula/#str-bool-bool) | Hämtar formeln för totalraden i den här listkolumnen.|
| [get_custom_calculated_formula(is_r1c1, is_local)](/cells/sv/python-net/aspose.cells.tables/listcolumn/get_custom_calculated_formula/#bool-bool) | Hämtar formeln för den här listkolumnen.|
| [set_custom_calculated_formula(formula, is_r1c1, is_local)](/cells/sv/python-net/aspose.cells.tables/listcolumn/set_custom_calculated_formula/#str-bool-bool) | Ställer in formeln för den här listkolumnen.|



###  Exempel

```python
from aspose.cells import CellsHelper, Workbook
from aspose.cells.tables import TotalsCalculation

workbook = Workbook()
cells = workbook.worksheets[0].cells
for i in range(5):
    cells.get(0, i).put_value(CellsHelper.column_index_to_name(i))
for row in range(1, 10):
    for column in range(4):
        cells.get(row, column).put_value(row * column)
tables = workbook.worksheets[0].list_objects
index = tables.add(0, 0, 9, 4, True)
table = tables[0]
table.show_totals = True
listColumn = table.list_columns[4]
listColumn.totals_calculation = TotalsCalculation.SUM
listColumn.formula = "=[A]"
workbook.save(r"Book1.xlsx")

```

###  Se även
* modul [aspose.cells.tables](..)
