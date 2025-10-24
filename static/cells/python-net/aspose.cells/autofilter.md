##AutoFilter class
## AutoFilter class
Represents autofiltering for the specified worksheet.
The AutoFilter type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [sorter](/cells/python-net/aspose.cells/autofilter/sorter) | Gets the data sorter. |
| [range](/cells/python-net/aspose.cells/autofilter/range) | Represents the range to which the specified AutoFilter applies. |
| [show_filter_button](/cells/python-net/aspose.cells/autofilter/show_filter_button) | Indicates whether the AutoFilter button for this column is visible. |
| [filter_columns](/cells/python-net/aspose.cells/autofilter/filter_columns) | Gets the collection of the filter columns. |
### Methods
| Method | Description |
| :- | :- |
| [`get_cell_area(self)`](/cells/python-net/aspose.cells/autofilter/get_cell_area/#) | Gets the [`CellArea`](/cells/python-net/aspose.cells/cellarea) where the this AutoFilter applies to. |
| [`get_cell_area(self, refresh_applied_range)`](/cells/python-net/aspose.cells/autofilter/get_cell_area/#bool) | Gets the [`CellArea`](/cells/python-net/aspose.cells/cellarea) where the specified AutoFilter applies to. |
| [`remove_filter(self, field_index, criteria)`](/cells/python-net/aspose.cells/autofilter/remove_filter/#int-system.string) | Removes a filter for a filter column. |
| [`remove_filter(self, field_index)`](/cells/python-net/aspose.cells/autofilter/remove_filter/#int) | Remove the specific filter. |
| [`custom(self, field_index, operator_type1, criteria1)`](/cells/python-net/aspose.cells/autofilter/custom/#int-aspose.cells.filteroperatortype-system.object) | Filters a list with a custom criteria. |
| [`custom(self, field_index, operator_type1, criteria1, is_and, operator_type2, criteria2)`](/cells/python-net/aspose.cells/autofilter/custom/#int-aspose.cells.filteroperatortype-system.object-bool-aspose.cells.filteroperatortype-system.object) | Filters a list with custom criteria. |
| [`refresh(self)`](/cells/python-net/aspose.cells/autofilter/refresh/#) | Refresh auto filters to hide or unhide the rows. |
| [`refresh(self, hide_rows)`](/cells/python-net/aspose.cells/autofilter/refresh/#bool) | Gets all hidden rows' indexes. |
| [`set_range(self, row, start_column, end_column)`](/cells/python-net/aspose.cells/autofilter/set_range/#int-int-int) | Sets the range to which the specified AutoFilter applies. |
| [`add_filter(self, field_index, criteria)`](/cells/python-net/aspose.cells/autofilter/add_filter/#int-system.string) | Adds a filter for a filter column. |
| [`add_date_filter(self, field_index, date_time_grouping_type, year, month, day, hour, minute, second)`](/cells/python-net/aspose.cells/autofilter/add_date_filter/#int-aspose.cells.datetimegroupingtype-int-int-int-int-int-int) | Adds a date filter. |
| [`remove_date_filter(self, field_index, date_time_grouping_type, year, month, day, hour, minute, second)`](/cells/python-net/aspose.cells/autofilter/remove_date_filter/#int-aspose.cells.datetimegroupingtype-int-int-int-int-int-int) | Removes a date filter. |
| [`filter(self, field_index, criteria)`](/cells/python-net/aspose.cells/autofilter/filter/#int-system.string) | Filters a list with specified criteria. |
| [`filter_top10(self, field_index, is_top, is_percent, item_count)`](/cells/python-net/aspose.cells/autofilter/filter_top10/#int-bool-bool-int) | Filter the top 10 item in the list |
| [`dynamic_filter(self, field_index, dynamic_filter_type)`](/cells/python-net/aspose.cells/autofilter/dynamic_filter/#int-aspose.cells.dynamicfiltertype) | Adds a dynamic filter. |
| [`add_font_color_filter(self, field_index, color)`](/cells/python-net/aspose.cells/autofilter/add_font_color_filter/#int-aspose.cells.cellscolor) | Adds a font color filter. |
| [`add_fill_color_filter(self, field_index, pattern, foreground_color, background_color)`](/cells/python-net/aspose.cells/autofilter/add_fill_color_filter/#int-aspose.cells.backgroundtype-aspose.cells.cellscolor-aspose.cells.cellscolor) | Adds a fill color filter. |
| [`add_icon_filter(self, field_index, icon_set_type, icon_id)`](/cells/python-net/aspose.cells/autofilter/add_icon_filter/#int-aspose.cells.iconsettype-int) | Adds an icon filter. |
| [`match_blanks(self, field_index)`](/cells/python-net/aspose.cells/autofilter/match_blanks/#int) | Match all blank cell in the list. |
| [`match_non_blanks(self, field_index)`](/cells/python-net/aspose.cells/autofilter/match_non_blanks/#int) | Match all not blank cell in the list. |
| [`show_all(self)`](/cells/python-net/aspose.cells/autofilter/show_all/#) | Unhide all rows. |
### Example
```python
from aspose.cells import Workbook
# Creating a file stream containing the Excel file to be opened
# Instantiating a Workbook object
workbook = Workbook("template.xlsx")
# Accessing the first worksheet in the Excel file
worksheet = workbook.worksheets[0]
# Creating AutoFilter by giving the cells range of the heading row
worksheet.auto_filter.range = "A1:B1"
# Filtering columns with specified values
worksheet.auto_filter.filter(1, "Bananas")
# Saving the modified Excel file.
workbook.save("output.xls")
```
### See Also
* module [`aspose.cells`](..)
* class [`CellArea`](/cells/python-net/aspose.cells/cellarea)
