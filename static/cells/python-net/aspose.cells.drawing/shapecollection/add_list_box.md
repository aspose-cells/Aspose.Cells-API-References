##add_list_box method
## add_list_box(self, upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Adds a ListBox to the worksheet.
### Returns
A ListBox object.
```python
def add_list_box(self, upper_left_row, top, upper_left_column, left, height, width):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| top | int | Represents the vertical  offset of ListBox from its left row, in unit of pixel. |
| upper_left_column | int | Upper left column index. |
| left | int | Represents the horizontal offset of ListBox from its left column, in unit of pixel. |
| height | int | Represents the height of ListBox, in unit of pixel. |
| width | int | Represents the width of ListBox, in unit of pixel. |
### Example
```python
# add a list box
listBox = shapes.add_list_box(1, 0, 1, 0, 100, 50)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`ListBox`](/cells/python-net/aspose.cells.drawing/listbox)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)
