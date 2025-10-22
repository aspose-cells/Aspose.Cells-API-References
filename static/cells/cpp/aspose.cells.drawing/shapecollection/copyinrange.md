##Aspose::Cells::Drawing::ShapeCollection::CopyInRange method
'Aspose::Cells::Drawing::ShapeCollection::CopyInRange method. Copy shapes in the range to destination range in C++.'
## ShapeCollection::CopyInRange method
Copy shapes in the range to destination range.
```cpp
void Aspose::Cells::Drawing::ShapeCollection::CopyInRange(const ShapeCollection &sourceShapes, const CellArea &ca, int32_t destRow, int32_t destColumn, bool isContained)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceShapes | const ShapeCollection\& | Source shapes. |
| ca | const CellArea\& | The source range. |
| destRow | int32_t | The dest row index of the dest range. |
| destColumn | int32_t | The dest column of the dest range. |
| isContained | bool | Whether only copy the shapes which are contained in the range. If true,only copies the shapes in the range. Otherwise,it works as MS Office. |
## Examples
```cpp
//add a shape
shapes.AddRectangle(2, 0, 2, 0, 130, 130);
CellArea area2;
area2.StartColumn = 1;
area2.StartRow = 1;
area2.EndColumn = 5;
area2.EndRow = 11;
//copy
shapes.CopyInRange(shapes, area2, 12, 1, false);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Class [CellArea](../../../aspose.cells/cellarea/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
