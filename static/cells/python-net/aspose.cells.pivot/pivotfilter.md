##PivotFilter class
## PivotFilter class
Represents a PivotFilter in PivotFilter Collection.
The PivotFilter type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [use_whole_day](/cells/python-net/aspose.cells.pivot/pivotfilter/use_whole_day) | Indicates whether uses whole days in its filtering criteria. |
| [auto_filter](/cells/python-net/aspose.cells.pivot/pivotfilter/auto_filter) | Gets the autofilter of the pivot filter. |
| [filter_type](/cells/python-net/aspose.cells.pivot/pivotfilter/filter_type) | Gets the autofilter type of the pivot filter. |
| [field_index](/cells/python-net/aspose.cells.pivot/pivotfilter/field_index) | Gets the index of source field which this pivot filter is applied to. |
| [filter_category](/cells/python-net/aspose.cells.pivot/pivotfilter/filter_category) | Gets the category of this filter. |
| [value1](/cells/python-net/aspose.cells.pivot/pivotfilter/value1) | Gets the string value1 of the label pivot filter. |
| [value2](/cells/python-net/aspose.cells.pivot/pivotfilter/value2) | Gets the string value2 of the label pivot filter. |
| [measure_fld_index](/cells/python-net/aspose.cells.pivot/pivotfilter/measure_fld_index) | Gets the measure field index of the pivot filter. |
| [value_field_index](/cells/python-net/aspose.cells.pivot/pivotfilter/value_field_index) | Gets the index of value field in the value region. |
| [measure_cube_field_index](/cells/python-net/aspose.cells.pivot/pivotfilter/measure_cube_field_index) | Specifies the index of the measure cube field.
| [member_property_field_index](/cells/python-net/aspose.cells.pivot/pivotfilter/member_property_field_index) | Gets the member property field index of the pivot filter. |
| [name](/cells/python-net/aspose.cells.pivot/pivotfilter/name) | Gets the name of the pivot filter. |
| [evaluation_order](/cells/python-net/aspose.cells.pivot/pivotfilter/evaluation_order) | Gets the Evaluation Order of the pivot filter. |
### Methods
| Method | Description |
| :- | :- |
| [`get_top_10_value(self)`](/cells/python-net/aspose.cells.pivot/pivotfilter/get_top_10_value/#) | Gets top 10 setting of the filter. |
| [`get_labels(self)`](/cells/python-net/aspose.cells.pivot/pivotfilter/get_labels/#) | Gets labels of the caption filter. |
| [`get_number_values(self)`](/cells/python-net/aspose.cells.pivot/pivotfilter/get_number_values/#) | Gets values of the number filter. |
| [`get_date_time_values(self)`](/cells/python-net/aspose.cells.pivot/pivotfilter/get_date_time_values/#) | Gets values of the number filter. |
### Example
```python
from aspose.cells import Workbook
from aspose.cells.pivot import PivotFieldType, PivotFilterType, PivotTableStyleType
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
# Add top 10 filter
pivot.base_fields[0].filter_top10(0, PivotFilterType.COUNT, False, 2)
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")
```
### See Also
* module [`aspose.cells.pivot`](..)
