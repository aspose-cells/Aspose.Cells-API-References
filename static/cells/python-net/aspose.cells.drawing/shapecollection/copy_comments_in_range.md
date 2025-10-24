##copy_comments_in_range method
## copy_comments_in_range(self, shapes, ca, dest_row, dest_column) {#aspose.cells.drawing.ShapeCollection-aspose.cells.CellArea-int-int}
Copy all comments in the range.
```python
def copy_comments_in_range(self, shapes, ca, dest_row, dest_column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| shapes | aspose.cells.drawing.ShapeCollection | The source shapes. |
| ca | aspose.cells.CellArea | The source range. |
| dest_row | int | The dest range start row. |
| dest_column | int | The dest range start column. |
### Example
```python
from aspose.cells import CellArea
comments = workbook.worksheets[0].comments
# Add comment to cell A1
commentIndex = comments.add(0, 0)
comment = comments[commentIndex]
comment.note = "First note."
comment.font.name = "Times New Roman"
# Add comment to cell B2
comments.add("B2")
comment = comments.get("B2")
comment.note = "Second note."
area1 = CellArea()
area1.start_column = 1
area1.start_row = 1
area1.end_column = 5
area1.end_row = 4
# copy
shapes.copy_comments_in_range(shapes, area1, 5, 1)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)
