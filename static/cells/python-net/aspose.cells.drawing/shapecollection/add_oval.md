##add_oval method
## add_oval(self, upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Adds a Oval to the worksheet.
### Returns
A Oval object.
```python
def add_oval(self, upper_left_row, top, upper_left_column, left, height, width):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| top | int | Represents the vertical  offset of Oval from its left row, in unit of pixel. |
| upper_left_column | int | Upper left column index. |
| left | int | Represents the horizontal offset of Oval from its left column, in unit of pixel. |
| height | int | Represents the height of Oval, in unit of pixel. |
| width | int | Represents the width of Oval, in unit of pixel. |
### Example
```python
# add a oval
oval = shapes.add_oval(1, 0, 1, 0, 50, 50)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`Oval`](/cells/python-net/aspose.cells.drawing/oval)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)
