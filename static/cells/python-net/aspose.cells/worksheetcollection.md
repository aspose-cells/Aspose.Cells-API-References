##WorksheetCollection class
## WorksheetCollection class
Encapsulates a collection of [`Worksheet`](/cells/python-net/aspose.cells/worksheet) objects.
The WorksheetCollection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [web_extension_task_panes](/cells/python-net/aspose.cells/worksheetcollection/web_extension_task_panes) | Gets the list of task panes. |
| [web_extensions](/cells/python-net/aspose.cells/worksheetcollection/web_extensions) | Gets the list of task panes. |
| [threaded_comment_authors](/cells/python-net/aspose.cells/worksheetcollection/threaded_comment_authors) | Gets the list of threaded comment authors. |
| [is_refresh_all_connections](/cells/python-net/aspose.cells/worksheetcollection/is_refresh_all_connections) | Indicates whether refresh all connections on opening file in MS Excel. |
| [names](/cells/python-net/aspose.cells/worksheetcollection/names) | Gets the collection of all the Name objects in the spreadsheet. |
| [active_sheet_name](/cells/python-net/aspose.cells/worksheetcollection/active_sheet_name) | Represents the name of active worksheet when the spreadsheet is opened. |
| [active_sheet_index](/cells/python-net/aspose.cells/worksheetcollection/active_sheet_index) | Represents the index of active worksheet when the spreadsheet is opened. |
| [dxfs](/cells/python-net/aspose.cells/worksheetcollection/dxfs) | Gets the master differential formatting records. |
| [xml_maps](/cells/python-net/aspose.cells/worksheetcollection/xml_maps) | Gets and sets the XML maps in the workbook. |
| [built_in_document_properties](/cells/python-net/aspose.cells/worksheetcollection/built_in_document_properties) | Returns a [`DocumentProperty`](/cells/python-net/aspose.cells.properties/documentproperty) collection that represents all the built-in document properties of the spreadsheet. |
| [custom_document_properties](/cells/python-net/aspose.cells/worksheetcollection/custom_document_properties) | Returns a [`DocumentProperty`](/cells/python-net/aspose.cells.properties/documentproperty) collection that represents all the custom document properties of the spreadsheet. |
| [ole_size](/cells/python-net/aspose.cells/worksheetcollection/ole_size) | Gets and Sets displayed size when Workbook file is used as an Ole object. |
| [external_links](/cells/python-net/aspose.cells/worksheetcollection/external_links) | Represents external links in a workbook. |
| [table_styles](/cells/python-net/aspose.cells/worksheetcollection/table_styles) | Gets [`WorksheetCollection.table_styles`](/cells/python-net/aspose.cells/worksheetcollection#table_styles) object. |
| [revision_logs](/cells/python-net/aspose.cells/worksheetcollection/revision_logs) | Represents revision logs. |
| [sensitivity_labels](/cells/python-net/aspose.cells/worksheetcollection/sensitivity_labels) | Represents all sensitivity labels. |
| [capacity](/cells/python-net/aspose.cells/worksheetcollection/capacity) | Gets or sets the number of elements that the array list can contain. |
Gets the [`Worksheet`](/cells/python-net/aspose.cells/worksheet) element at the specified index.
### Indexer
| Name | Description |
| :- | :- |
| [index] | The zero based index of the element. |
### Methods
| Method | Description |
| :- | :- |
| [`get(self, index)`](/cells/python-net/aspose.cells/worksheetcollection/get/#int) | Add API for Python Via .Net.since this[int index] is unsupported |
| [`get(self, sheet_name)`](/cells/python-net/aspose.cells/worksheetcollection/get/#system.string) | Add API for Python Via .Net.since this[string sheetName] is unsupported |
| [`add(self, type)`](/cells/python-net/aspose.cells/worksheetcollection/add/#aspose.cells.sheettype) | Adds a worksheet to the collection. |
| [`add(self)`](/cells/python-net/aspose.cells/worksheetcollection/add/#) | Adds a worksheet to the collection. |
| [`add(self, sheet_name)`](/cells/python-net/aspose.cells/worksheetcollection/add/#system.string) | Adds a worksheet to the collection. |
| [`register_add_in_function(self, add_in_file, function_name, lib)`](/cells/python-net/aspose.cells/worksheetcollection/register_add_in_function/#system.string-system.string-bool) | Adds addin function into the workbook |
| [`register_add_in_function(self, id, function_name)`](/cells/python-net/aspose.cells/worksheetcollection/register_add_in_function/#int-system.string) | Adds addin function into the workbook |
| [`add_copy(self, sheet_name)`](/cells/python-net/aspose.cells/worksheetcollection/add_copy/#system.string) | Adds a worksheet to the collection and copies data from an existed worksheet. |
| [`add_copy(self, sheet_index)`](/cells/python-net/aspose.cells/worksheetcollection/add_copy/#int) | Adds a worksheet to the collection and copies data from an existed worksheet. |
| [`add_copy(self, source, dest_sheet_names)`](/cells/python-net/aspose.cells/worksheetcollection/add_copy/#list-list) | Copy a group of worksheets. |
| [`get_range_by_name(self, range_name)`](/cells/python-net/aspose.cells/worksheetcollection/get_range_by_name/#system.string) | Gets Range object by pre-defined name. |
| [`get_range_by_name(self, range_name, current_sheet_index, include_table)`](/cells/python-net/aspose.cells/worksheetcollection/get_range_by_name/#system.string-int-bool) | Gets [`Range`](/cells/python-net/aspose.cells/range) by pre-defined name or table's name |
| [`refresh_pivot_tables(self)`](/cells/python-net/aspose.cells/worksheetcollection/refresh_pivot_tables/#) | Refreshes all the PivotTables in the Excel file. |
| [`refresh_pivot_tables(self, option)`](/cells/python-net/aspose.cells/worksheetcollection/refresh_pivot_tables/#aspose.cells.pivot.pivottablerefreshoption) | Refreshes all the PivotTables in the Excel file. |
| [`copy_to(self, array)`](/cells/python-net/aspose.cells/worksheetcollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [`copy_to(self, index, array, array_index, count)`](/cells/python-net/aspose.cells/worksheetcollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [`index_of(self, item, index)`](/cells/python-net/aspose.cells/worksheetcollection/index_of/#aspose.cells.worksheet-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [`index_of(self, item, index, count)`](/cells/python-net/aspose.cells/worksheetcollection/index_of/#aspose.cells.worksheet-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [`last_index_of(self, item)`](/cells/python-net/aspose.cells/worksheetcollection/last_index_of/#aspose.cells.worksheet) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [`last_index_of(self, item, index)`](/cells/python-net/aspose.cells/worksheetcollection/last_index_of/#aspose.cells.worksheet-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [`last_index_of(self, item, index, count)`](/cells/python-net/aspose.cells/worksheetcollection/last_index_of/#aspose.cells.worksheet-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [`create_range(self, address, sheet_index)`](/cells/python-net/aspose.cells/worksheetcollection/create_range/#system.string-int) | Creates a [`Range`](/cells/python-net/aspose.cells/range) object from an address of the range. |
| [`create_union_range(self, address, sheet_index)`](/cells/python-net/aspose.cells/worksheetcollection/create_union_range/#system.string-int) | Creates a [`Range`](/cells/python-net/aspose.cells/range) object from an address of the range. |
| [`get_sheet_by_code_name(self, code_name)`](/cells/python-net/aspose.cells/worksheetcollection/get_sheet_by_code_name/#system.string) | Gets the worksheet by the code name. |
| [`sort_names(self)`](/cells/python-net/aspose.cells/worksheetcollection/sort_names/#) | Sorts the defined names. |
| [`swap_sheet(self, sheet_index1, sheet_index2)`](/cells/python-net/aspose.cells/worksheetcollection/swap_sheet/#int-int) | Swaps the two sheets. |
| [`remove_by_name(self, name)`](/cells/python-net/aspose.cells/worksheetcollection/remove_by_name/#system.string) | Remove a sheet by sheet name.(CELLSPYTHONNET-192) |
| [`remove_by_index(self, index)`](/cells/python-net/aspose.cells/worksheetcollection/remove_by_index/#int) | Remove a sheet by sheet index |
| [`remove_at(self, name)`](/cells/python-net/aspose.cells/worksheetcollection/remove_at/#system.string) | Removes the element at a specified name. |
| [`get_named_ranges(self)`](/cells/python-net/aspose.cells/worksheetcollection/get_named_ranges/#) | Gets all pre-defined named ranges in the spreadsheet. |
| [`get_named_ranges_and_tables(self)`](/cells/python-net/aspose.cells/worksheetcollection/get_named_ranges_and_tables/#) | Gets all pre-defined named ranges in the spreadsheet. |
| [`set_ole_size(self, start_row, end_row, start_column, end_column)`](/cells/python-net/aspose.cells/worksheetcollection/set_ole_size/#int-int-int-int) | Sets displayed size when Workbook file is used as an Ole object. |
| [`clear_pivottables(self)`](/cells/python-net/aspose.cells/worksheetcollection/clear_pivottables/#) | Clears pivot tables from the spreadsheet. |
| [`refresh_all(self)`](/cells/python-net/aspose.cells/worksheetcollection/refresh_all/#) | Refresh all pivot tables and charts with pivot source. |
| [`binary_search(self, item)`](/cells/python-net/aspose.cells/worksheetcollection/binary_search/#aspose.cells.worksheet) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |
### Example
```python
from aspose.cells import Workbook
workbook = Workbook()
sheets = workbook.worksheets
# Add a worksheet
sheets.add()
# Change the name of a worksheet
sheets[0].name = "First Sheet"
# Set the active sheet to the second worksheet
sheets.active_sheet_index = 1
```
### See Also
* module [`aspose.cells`](..)
* class [`DocumentProperty`](/cells/python-net/aspose.cells.properties/documentproperty)
* class [`Range`](/cells/python-net/aspose.cells/range)
* class [`Worksheet`](/cells/python-net/aspose.cells/worksheet)
