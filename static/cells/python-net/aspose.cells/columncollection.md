##ColumnCollection class
## ColumnCollection class
Collection of the [`Column`](/cells/python-net/aspose.cells/column) objects that represent the individual column(setting)s in a worksheet.
The Column object only represents the settings such as column width, styles, .etc. for the whole column,
has nothing to do with the fact that there are non-empty cells(data) or not in corresponding column.
And the "Count" of this collection only represents the count Column objects that have been instantiated in this collection,
has nothing to do with the fact that there are non-empty cells(data) or not in the worksheet.
The ColumnCollection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [capacity](/cells/python-net/aspose.cells/columncollection/capacity) | Gets or sets the number of elements that the array list can contain. |
### Methods
| Method | Description |
| :- | :- |
| [`copy_to(self, array)`](/cells/python-net/aspose.cells/columncollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [`copy_to(self, index, array, array_index, count)`](/cells/python-net/aspose.cells/columncollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [`index_of(self, item, index)`](/cells/python-net/aspose.cells/columncollection/index_of/#aspose.cells.column-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [`index_of(self, item, index, count)`](/cells/python-net/aspose.cells/columncollection/index_of/#aspose.cells.column-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [`last_index_of(self, item)`](/cells/python-net/aspose.cells/columncollection/last_index_of/#aspose.cells.column) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [`last_index_of(self, item, index)`](/cells/python-net/aspose.cells/columncollection/last_index_of/#aspose.cells.column-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [`last_index_of(self, item, index, count)`](/cells/python-net/aspose.cells/columncollection/last_index_of/#aspose.cells.column-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [`get_by_index(self, index)`](/cells/python-net/aspose.cells/columncollection/get_by_index/#int) | Gets the column object by the index. |
| [`get_column_by_index(self, index)`](/cells/python-net/aspose.cells/columncollection/get_column_by_index/#int) | Gets the [`Column`](/cells/python-net/aspose.cells/column) object by the position in the list. |
| [`get(self, column_index)`](/cells/python-net/aspose.cells/columncollection/get/#int) | Add API for Python Via .Net. |
| [`binary_search(self, item)`](/cells/python-net/aspose.cells/columncollection/binary_search/#aspose.cells.column) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |
### Example
```python
from aspose.cells import BackgroundType, StyleFlag, Workbook
from aspose.pydrawing import Color
# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Add new Style to Workbook
style = workbook.create_style()
# Setting the background color to Blue
style.foreground_color = Color.blue
# setting Background Pattern
style.pattern = BackgroundType.SOLID
# New Style Flag
styleFlag = StyleFlag()
# Set All Styles
styleFlag.all = True
# Change the default width of first ten columns
for i in range(10):
worksheet.cells.columns[i].width = 20.0
# Get the Column with non default formatting
columns = worksheet.cells.columns
for column in columns:
# Apply Style to first ten Columns
column.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")
```
### See Also
* module [`aspose.cells`](..)
* class [`Column`](/cells/python-net/aspose.cells/column)
