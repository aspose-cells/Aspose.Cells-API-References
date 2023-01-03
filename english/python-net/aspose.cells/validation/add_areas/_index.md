---
title: add_areas method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 30
url: /python-net/aspose.cells/validation/add_areas/
is_root: false
---

## add_areas(areas, check_intersection, check_edge) {#list-bool-bool}

Applies the validation to given areas.



```python
def add_areas(self, areas, check_intersection, check_edge):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| areas | list | The areas. |
| check_intersection | bool | Whether check the intersection of given area with existing validations' areas.<br/>If one validation has been applied in given area(or part of it),<br/>then the existing validation should be removed at first from given area.<br/>Otherwise corruption may be caused for the generated Validations.<br/>If user is sure that all the added areas do not intersect with any existing area,<br/>this parameter can be set as false for performance consideration. |
| check_edge | bool | Whether check the edge of this validation's applied areas.<br/>Validation's internal settings depend on the top-left one of its applied ranges,<br/>so if one of given areas will become the new top-left one of the applied ranges,<br/>the internal settings should be changed and rebuilt, otherwise unexpected result may be caused.<br/>If user is sure that no one of those added areas is the top-left,<br/>this parameter can be set as false for performance consideration. |
### Remarks

In this method, we will remove all old validations in given area.
For the top-left one of Validation's applied ranges, firstly its StartRow is smallest,
secondly its StartColumn is the smallest one of those areas who have the same smallest StartRow.


### See Also
* module [aspose.cells](../../)
* class [Validation](/cells/python-net/aspose.cells/validation)
