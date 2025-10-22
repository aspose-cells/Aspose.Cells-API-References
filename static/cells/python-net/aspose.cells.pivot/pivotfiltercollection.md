##PivotFilterCollection class
## PivotFilterCollection class
Represents a collection of all the PivotFilter objects
The PivotFilterCollection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [capacity](/cells/python-net/aspose.cells.pivot/pivotfiltercollection/capacity) | Gets or sets the number of elements that the array list can contain. |
### Methods
| Method | Description |
| :- | :- |
| [`copy_to(self, array)`](/cells/python-net/aspose.cells.pivot/pivotfiltercollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [`copy_to(self, index, array, array_index, count)`](/cells/python-net/aspose.cells.pivot/pivotfiltercollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [`index_of(self, item, index)`](/cells/python-net/aspose.cells.pivot/pivotfiltercollection/index_of/#aspose.cells.pivot.pivotfilter-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [`index_of(self, item, index, count)`](/cells/python-net/aspose.cells.pivot/pivotfiltercollection/index_of/#aspose.cells.pivot.pivotfilter-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [`last_index_of(self, item)`](/cells/python-net/aspose.cells.pivot/pivotfiltercollection/last_index_of/#aspose.cells.pivot.pivotfilter) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [`last_index_of(self, item, index)`](/cells/python-net/aspose.cells.pivot/pivotfiltercollection/last_index_of/#aspose.cells.pivot.pivotfilter-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [`last_index_of(self, item, index, count)`](/cells/python-net/aspose.cells.pivot/pivotfiltercollection/last_index_of/#aspose.cells.pivot.pivotfilter-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [`add(self, field_index, type)`](/cells/python-net/aspose.cells.pivot/pivotfiltercollection/add/#int-aspose.cells.pivot.pivotfiltertype) | Adds a PivotFilter Object to the specific type |
| [`add_top_10_filter(self, base_field_index, value_field_index, type, is_top, item_count)`](/cells/python-net/aspose.cells.pivot/pivotfiltercollection/add_top_10_filter/#int-int-aspose.cells.pivot.pivotfiltertype-bool-int) | Filters by values of data pivot field. |
| [`add_value_filter(self, base_field_index, value_field_index, type, value1, value2)`](/cells/python-net/aspose.cells.pivot/pivotfiltercollection/add_value_filter/#int-int-aspose.cells.pivot.pivotfiltertype-float-float) | Filters by values of data pivot field. |
| [`add_label_filter(self, base_field_index, type, label1, label2)`](/cells/python-net/aspose.cells.pivot/pivotfiltercollection/add_label_filter/#int-aspose.cells.pivot.pivotfiltertype-system.string-system.string) | Filters by captions of row or column pivot field. |
| [`add_date_filter(self, base_field_index, type, date_time1, date_time2)`](/cells/python-net/aspose.cells.pivot/pivotfiltercollection/add_date_filter/#int-aspose.cells.pivot.pivotfiltertype-system.datetime-system.datetime) | Filters by date setting of row or column pivot field. |
| [`clear_filter(self, field_index)`](/cells/python-net/aspose.cells.pivot/pivotfiltercollection/clear_filter/#int) | Clear PivotFilter from the specific PivotField |
| [`binary_search(self, item)`](/cells/python-net/aspose.cells.pivot/pivotfiltercollection/binary_search/#aspose.cells.pivot.pivotfilter) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |
### See Also
* module [`aspose.cells.pivot`](..)
