##ListColumn class
## ListColumn class
Represents a column in a Table.
The ListColumn type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [name](/cells/python-net/aspose.cells.tables/listcolumn/name) | Gets and sets the name of the column. |
| [totals_calculation](/cells/python-net/aspose.cells.tables/listcolumn/totals_calculation) | Gets and sets the type of calculation in the Totals row of the list column. |
| [range](/cells/python-net/aspose.cells.tables/listcolumn/range) | Gets the range of this list column. |
| [is_array_formula](/cells/python-net/aspose.cells.tables/listcolumn/is_array_formula) | Indicates whether the fomula is array formula. |
| [formula](/cells/python-net/aspose.cells.tables/listcolumn/formula) | Gets and sets the formula of the list column. |
| [totals_row_label](/cells/python-net/aspose.cells.tables/listcolumn/totals_row_label) | Gets and sets the display labels of total row. |
### Methods
| Method | Description |
| :- | :- |
| [`get_custom_totals_row_formula(self, is_r1c1, is_local)`](/cells/python-net/aspose.cells.tables/listcolumn/get_custom_totals_row_formula/#bool-bool) | Gets the formula of totals row of this list column. |
| [`set_custom_totals_row_formula(self, formula, is_r1c1, is_local)`](/cells/python-net/aspose.cells.tables/listcolumn/set_custom_totals_row_formula/#system.string-bool-bool) | Gets the formula of totals row of this list column. |
| [`get_custom_calculated_formula(self, is_r1c1, is_local)`](/cells/python-net/aspose.cells.tables/listcolumn/get_custom_calculated_formula/#bool-bool) | Gets the formula of this list column. |
| [`set_custom_calculated_formula(self, formula, is_r1c1, is_local)`](/cells/python-net/aspose.cells.tables/listcolumn/set_custom_calculated_formula/#system.string-bool-bool) | Sets the formula for this list column. |
| [`get_data_style(self)`](/cells/python-net/aspose.cells.tables/listcolumn/get_data_style/#) | Gets the style of the data in this column of the table. |
| [`set_data_style(self, style)`](/cells/python-net/aspose.cells.tables/listcolumn/set_data_style/#aspose.cells.style) | Sets the style of the data in this column of the table. |
### Example
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
### See Also
* module [`aspose.cells.tables`](..)
