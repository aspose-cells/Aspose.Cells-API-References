##Aspose::Cells::Drawing::ShapeCollection::DeleteInRange method
'Aspose::Cells::Drawing::ShapeCollection::DeleteInRange method. Delete shapes in the range.Comment shapes will not be deleted in C++.'
## ShapeCollection::DeleteInRange method
Delete shapes in the range.Comment shapes will not be deleted.
```cpp
void Aspose::Cells::Drawing::ShapeCollection::DeleteInRange(const CellArea &ca)
```
| Parameter | Type | Description |
| --- | --- | --- |
| ca | const CellArea\& | The range.If the shapes are contained in the range, they will be removed. |
## Examples
```cpp
//add first shape
shapes.AddRectangle(2, 0, 2, 0, 50, 50);
//add second shape
shapes.AddRectangle(6, 0, 2, 0, 30, 30);
CellArea area3;
area3.StartColumn = 0;
area3.StartRow = 5;
area3.EndColumn = 5;
area3.EndRow = 8;
//del
shapes.DeleteInRange(area3);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [CellArea](../../../aspose.cells/cellarea/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
