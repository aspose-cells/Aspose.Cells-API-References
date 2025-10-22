##PivotTableCollection class
## PivotTableCollection class
Represents the collection of all the PivotTable objects on the specified worksheet.
The PivotTableCollection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [capacity](/cells/python-net/aspose.cells.pivot/pivottablecollection/capacity) | Gets or sets the number of elements that the array list can contain. |
### Methods
| Method | Description |
| :- | :- |
| [`add(self, source_data, dest_cell_name, table_name)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/add/#system.string-system.string-system.string) | Adds a new PivotTable. |
| [`add(self, source_data, dest_cell_name, table_name, use_same_source)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/add/#system.string-system.string-system.string-bool) | Adds a new PivotTable. |
| [`add(self, source_data, row, column, table_name)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/add/#system.string-int-int-system.string) | Adds a new PivotTable. |
| [`add(self, source_data, row, column, table_name, use_same_source)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/add/#system.string-int-int-system.string-bool) | Adds a new PivotTable. |
| [`add(self, source_data, row, column, table_name, use_same_source, is_xls_classic)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/add/#system.string-int-int-system.string-bool-bool) | Adds a new PivotTable. |
| [`add(self, source_data, cell, table_name, use_same_source, is_xls_classic)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/add/#system.string-system.string-system.string-bool-bool) | Adds a new PivotTable. |
| [`add(self, pivot_table, dest_cell_name, table_name)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/add/#aspose.cells.pivot.pivottable-system.string-system.string) | Adds a new PivotTable based on another PivotTable. |
| [`add(self, pivot_table, row, column, table_name)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/add/#aspose.cells.pivot.pivottable-int-int-system.string) | Adds a new PivotTable based on another PivotTable. |
| [`add(self, source_data, is_auto_page, page_fields, dest_cell_name, table_name)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/add/#list-bool-aspose.cells.pivot.pivotpagefields-system.string-system.string) | Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source. |
| [`add(self, source_data, is_auto_page, page_fields, row, column, table_name)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/add/#list-bool-aspose.cells.pivot.pivotpagefields-int-int-system.string) | Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source. |
| [`copy_to(self, array)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [`copy_to(self, index, array, array_index, count)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [`index_of(self, item, index)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/index_of/#aspose.cells.pivot.pivottable-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [`index_of(self, item, index, count)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/index_of/#aspose.cells.pivot.pivottable-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [`last_index_of(self, item)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/last_index_of/#aspose.cells.pivot.pivottable) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [`last_index_of(self, item, index)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/last_index_of/#aspose.cells.pivot.pivottable-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [`last_index_of(self, item, index, count)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/last_index_of/#aspose.cells.pivot.pivottable-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [`get(self, name)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/get/#system.string) | Gets the PivotTable report by pivottable's name. |
| [`remove_pivot_table(self, pivot_table)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/remove_pivot_table/#aspose.cells.pivot.pivottable) | Deletes the specified PivotTable and delete the PivotTable data |
| [`remove_pivot_table_data(self, pivot_table, keep_data)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/remove_pivot_table_data/#aspose.cells.pivot.pivottable-bool) | Deletes the specified PivotTable |
| [`remove_by_index(self, index)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/remove_by_index/#int) | Deletes the PivotTable at the specified index and delete the PivotTable data |
| [`remove_at(self, index, keep_data)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/remove_at/#int-bool) | Deletes the PivotTable at the specified index |
| [`binary_search(self, item)`](/cells/python-net/aspose.cells.pivot/pivottablecollection/binary_search/#aspose.cells.pivot.pivottable) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |
### Example
```python
from aspose.cells import FormatConditionType, OperatorType, Workbook
from aspose.cells.pivot import PivotFieldType, PivotFilterType, PivotTableStyleType
from aspose.pydrawing import Color
book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
cells.get(5, 0).value = "grape"
cells.get(6, 0).value = "blueberry"
cells.get(7, 0).value = "kiwi"
cells.get(8, 0).value = "cherry"
cells.get(0, 1).value = "year"
cells.get(1, 1).value = 2020
cells.get(2, 1).value = 2020
cells.get(3, 1).value = 2020
cells.get(4, 1).value = 2020
cells.get(5, 1).value = 2021
cells.get(6, 1).value = 2021
cells.get(7, 1).value = 2021
cells.get(8, 1).value = 2021
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
cells.get(5, 2).value = 90
cells.get(6, 2).value = 100
cells.get(7, 2).value = 110
cells.get(8, 2).value = 120
pivots = sheet.pivot_tables
pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "year")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
# Change PivotField's attributes
rowField = pivot.row_fields[0]
rowField.display_name = "custom display name"
# Add PivotFilter
index = pivot.pivot_filters.add(0, PivotFilterType.COUNT)
filter = pivot.pivot_filters[index]
filter.auto_filter.filter_top10(0, False, False, 2)
# Add PivotFormatCondition
formatIndex = pivot.pivot_format_conditions.add()
pfc = pivot.pivot_format_conditions[formatIndex]
fcc = pfc.format_conditions
fcc.add_area(pivot.data_body_range)
idx = fcc.add_condition(FormatConditionType.CELL_VALUE)
fc = fcc[idx]
fc.formula1 = "100"
fc.operator = OperatorType.GREATER_OR_EQUAL
fc.style.background_color = Color.red
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")
```
### See Also
* module [`aspose.cells.pivot`](..)
