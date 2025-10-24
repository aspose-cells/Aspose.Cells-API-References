##add_areas method
## add_areas(self, areas, check_intersection, check_edge) {#list-bool-bool}
Applies the validation to given areas.
```python
def add_areas(self, areas, check_intersection, check_edge):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| areas | list | The areas. |
| check_intersection | bool | Whether check the intersection of given area with existing validations' areas.
| check_edge | bool | Whether check the edge of this validation's applied areas.
### Remarks
In this method, we will remove all old validations in given area.
For the top-left one of Validation's applied ranges, firstly its StartRow is smallest,
secondly its StartColumn is the smallest one of those areas who have the same smallest StartRow.
### See Also
* module [`aspose.cells`](../../)
* class [`Validation`](/cells/python-net/aspose.cells/validation)
