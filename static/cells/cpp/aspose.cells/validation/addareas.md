##Aspose::Cells::Validation::AddAreas method
'Aspose::Cells::Validation::AddAreas method. Applies the validation to given areas in C++.'
## Validation::AddAreas method
Applies the validation to given areas.
```cpp
void Aspose::Cells::Validation::AddAreas(const Vector<CellArea> &areas, bool checkIntersection, bool checkEdge)
```
| Parameter | Type | Description |
| --- | --- | --- |
| areas | const Vector \<CellArea\>\& | The areas. |
| checkIntersection | bool | Whether check the intersection of given area with existing validations' areas. If one validation has been applied in given area(or part of it), then the existing validation should be removed at first from given area. Otherwise corruption may be caused for the generated Validations. If user is sure that all the added areas do not intersect with any existing area, this parameter can be set as false for performance consideration. |
| checkEdge | bool | Whether check the edge of this validation's applied areas. [Validation](../)'s internal settings depend on the top-left one of its applied ranges, so if one of given areas will become the new top-left one of the applied ranges, the internal settings should be changed and rebuilt, otherwise unexpected result may be caused. If user is sure that no one of those added areas is the top-left, this parameter can be set as false for performance consideration. |
## Remarks
In this method, we will remove all old validations in given area. For the top-left one of [Validation](../)'s applied ranges, firstly its StartRow is smallest, secondly its StartColumn is the smallest one of those areas who have the same smallest StartRow.
## See Also
* Class [Vector](../../vector/)
* Class [CellArea](../../cellarea/)
* Class [Validation](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
