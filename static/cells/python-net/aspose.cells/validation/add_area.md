##add_area method
## add_area(self, cell_area) {#aspose.cells.CellArea}
Applies the validation to the area.
```python
def add_area(self, cell_area):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| cell_area | aspose.cells.CellArea | The area. |
### Remarks
It is equivalent to use [`Validation.add_area`](/cells/python-net/aspose.cells/validation/add_area)
with checking intersection and edge.
## add_area(self, cell_area, check_intersection, check_edge) {#aspose.cells.CellArea-bool-bool}
Applies the validation to the area.
```python
def add_area(self, cell_area, check_intersection, check_edge):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| cell_area | aspose.cells.CellArea | The area. |
| check_intersection | bool | Whether check the intersection of given area with existing validations' areas.
| check_edge | bool | Whether check the edge of this validation's applied areas.
### Remarks
In this method, we will remove all old validations in given area.
For the top-left one of Validation's applied ranges, firstly its StartRow is smallest,
secondly its StartColumn is the smallest one of those areas who have the same smallest StartRow.
### See Also
* module [`aspose.cells`](../../)
* class [`Validation`](/cells/python-net/aspose.cells/validation)
