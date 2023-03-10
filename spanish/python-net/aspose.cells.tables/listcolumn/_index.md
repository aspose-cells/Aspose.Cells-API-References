---
title: ListColumn clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 10
url: /es/python-net/aspose.cells.tables/listcolumn/
is_root: false
---
##  ListColumn clase
Representa una columna en una lista.



El tipo ListColumn expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [name](/cells/es/python-net/aspose.cells.tables/listcolumn/name) | Obtiene y establece el nombre de la columna.|
| [totals_calculation](/cells/es/python-net/aspose.cells.tables/listcolumn/totals_calculation) | Obtiene y establece el tipo de cálculo en la fila Totales de la columna de lista.|
| [range](/cells/es/python-net/aspose.cells.tables/listcolumn/range) | Obtiene el rango de esta columna de lista.|
| [formula](/cells/es/python-net/aspose.cells.tables/listcolumn/formula) | Obtiene y establece la fórmula de la columna de lista.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [get_custom_totals_row_formula(is_r1c1, is_local)](/cells/es/python-net/aspose.cells.tables/listcolumn/get_custom_totals_row_formula/#bool-bool) | Obtiene la fórmula de la fila de totales de esta columna de lista.|
| [set_custom_totals_row_formula(formula, is_r1c1, is_local)](/cells/es/python-net/aspose.cells.tables/listcolumn/set_custom_totals_row_formula/#str-bool-bool) | Obtiene la fórmula de la fila de totales de esta columna de lista.|
| [get_custom_calculated_formula(is_r1c1, is_local)](/cells/es/python-net/aspose.cells.tables/listcolumn/get_custom_calculated_formula/#bool-bool) | Obtiene la fórmula de esta columna de lista.|
| [set_custom_calculated_formula(formula, is_r1c1, is_local)](/cells/es/python-net/aspose.cells.tables/listcolumn/set_custom_calculated_formula/#str-bool-bool) | Establece la fórmula para esta columna de lista.|



###  Ejemplo

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

###  Ver también
* módulo [aspose.cells.tables](..)
