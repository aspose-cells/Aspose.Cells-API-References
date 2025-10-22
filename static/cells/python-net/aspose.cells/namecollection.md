##NameCollection class
## NameCollection class
Represents a collection of all the [`Name`](/cells/python-net/aspose.cells/name) objects in the spreadsheet.
The NameCollection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [capacity](/cells/python-net/aspose.cells/namecollection/capacity) | Gets or sets the number of elements that the array list can contain. |
### Methods
| Method | Description |
| :- | :- |
| [`get(self, index)`](/cells/python-net/aspose.cells/namecollection/get/#int) | Add API for Python Via .Net.since this[int index] is unsupported |
| [`get(self, text)`](/cells/python-net/aspose.cells/namecollection/get/#system.string) | Add API for Python Via .Net.since this[string text] is unsupported |
| [`copy_to(self, array)`](/cells/python-net/aspose.cells/namecollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [`copy_to(self, index, array, array_index, count)`](/cells/python-net/aspose.cells/namecollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [`index_of(self, item, index)`](/cells/python-net/aspose.cells/namecollection/index_of/#aspose.cells.name-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [`index_of(self, item, index, count)`](/cells/python-net/aspose.cells/namecollection/index_of/#aspose.cells.name-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [`last_index_of(self, item)`](/cells/python-net/aspose.cells/namecollection/last_index_of/#aspose.cells.name) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [`last_index_of(self, item, index)`](/cells/python-net/aspose.cells/namecollection/last_index_of/#aspose.cells.name-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [`last_index_of(self, item, index, count)`](/cells/python-net/aspose.cells/namecollection/last_index_of/#aspose.cells.name-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [`add(self, text)`](/cells/python-net/aspose.cells/namecollection/add/#system.string) | Defines a new name. |
| [`filter(self, type, sheet_index)`](/cells/python-net/aspose.cells/namecollection/filter/#aspose.cells.namescopetype-int) | Gets all defined name by scope. |
| [`remove_a_name(self, text)`](/cells/python-net/aspose.cells/namecollection/remove_a_name/#system.string) | Remove the name. |
| [`remove_names_by_array(self, names)`](/cells/python-net/aspose.cells/namecollection/remove_names_by_array/#list) | Remove an array of name |
| [`remove_duplicate_names(self)`](/cells/python-net/aspose.cells/namecollection/remove_duplicate_names/#) | Remove the duplicate defined names |
| [`binary_search(self, item)`](/cells/python-net/aspose.cells/namecollection/binary_search/#aspose.cells.name) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |
### See Also
* module [`aspose.cells`](..)
* class [`Name`](/cells/python-net/aspose.cells/name)
