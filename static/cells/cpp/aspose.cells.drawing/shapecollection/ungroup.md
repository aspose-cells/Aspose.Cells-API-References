##Aspose::Cells::Drawing::ShapeCollection::Ungroup method
'Aspose::Cells::Drawing::ShapeCollection::Ungroup method. Ungroups the shape items in C++.'
## ShapeCollection::Ungroup method
Ungroups the shape items.
```cpp
void Aspose::Cells::Drawing::ShapeCollection::Ungroup(const GroupShape &group)
```
| Parameter | Type | Description |
| --- | --- | --- |
| group | const GroupShape\& | The group shape. |
## Remarks
If the group shape is grouped by another group shape,nothing will be done.
## Examples
```cpp
//add first shape
shapes.AddRectangle(2, 0, 2, 0, 50, 50);
//add second shape
shapes.AddRectangle(6, 0, 2, 0, 30, 30);
//group
Vector<Shape> shapesArr{ shapes.Get(0), shapes.Get(1) };
GroupShape groupShape = shapes.Group(shapesArr);
//ungroup
shapes.Ungroup(groupShape);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [GroupShape](../../groupshape/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
