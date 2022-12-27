---
title: add_area method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 20
url: /python-net/aspose.cells/validation/add_area/
is_root: false
---

## add_area(cell_area) {#CellArea}

Applies the validation to the area.



```python
def add_area(self, cell_area):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| cell_area | [CellArea](/cells/python-net/aspose.cells/cellarea) | The area. |
### Remarks

It is equivalent to use [Validation.add_area(cell_area)](/cells/python-net/aspose.cells/validation/add_area)
with checking intersection and edge.

## add_area(cell_area, check_intersection, check_edge) {#CellArea-bool-bool}

Applies the validation to the area.



```python
def add_area(self, cell_area, check_intersection, check_edge):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| cell_area | [CellArea](/cells/python-net/aspose.cells/cellarea) | The area. |
| check_intersection | bool | Whether check the intersection of given area with existing validations' areas.<br/>If one validation has been applied in given area(or part of it),<br/>then the existing validation should be removed at first from given area.<br/>Otherwise corruption may be caused for the generated Validations.<br/>If user is sure that the added area does not intersect with any existing area,<br/>this parameter can be set as false for performance consideration. |
| check_edge | bool | Whether check the edge of this validation's applied areas.<br/>Validation's internal settings depend on the top-left one of its applied ranges,<br/>so if given area will become the new top-left one of the applied ranges,<br/>the internal settings should be changed and rebuilt, otherwise unexpected result may be caused.<br/>If user is sure that the added area is not the top-left one,<br/>this parameter can be set as false for performance consideration. |
### Remarks

In this method, we will remove all old validations in given area.
For the top-left one of Validation's applied ranges, firstly its StartRow is smallest,
secondly its StartColumn is the smallest one of those areas who have the same smallest StartRow.


### See Also
* module [aspose.cells](../../)
* class [Validation](/cells/python-net/aspose.cells/validation)
