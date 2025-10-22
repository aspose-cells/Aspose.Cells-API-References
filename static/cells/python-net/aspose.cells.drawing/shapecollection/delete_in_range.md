##delete_in_range method
## delete_in_range(self, ca) {#aspose.cells.CellArea}
Delete shapes in the range.Comment shapes will not be deleted.
```python
def delete_in_range(self, ca):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| ca | aspose.cells.CellArea | The range.If the shapes are contained in the range, they will be removed. |
### Example
```python
from aspose.cells import CellArea
# add first shape
shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
shapes.add_rectangle(6, 0, 2, 0, 30, 30)
area3 = CellArea()
area3.start_column = 0
area3.start_row = 5
area3.end_column = 5
area3.end_row = 8
# del
shapes.delete_in_range(area3)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)
