##Aspose::Cells::Drawing::ShapeCollection::Group method
'Aspose::Cells::Drawing::ShapeCollection::Group method. Group the shapes in C++.'
## ShapeCollection::Group method
Group the shapes.
```cpp
GroupShape Aspose::Cells::Drawing::ShapeCollection::Group(const Vector<Shape> &groupItems)
```
| Parameter | Type | Description |
| --- | --- | --- |
| groupItems | const Vector \<Shape\>\& | the group items. |
## ReturnValue
Return the group shape.
## Remarks
The shape in the groupItems should not be grouped. The shape must be in this Shapes collection.
## Examples
```cpp
//add first shape
shapes.AddRectangle(2, 0, 2, 0, 50, 50);
//add second shape
shapes.AddRectangle(6, 0, 2, 0, 30, 30);
Vector<Shape> shapesArr{ shapes.Get(0), shapes.Get(1) };
GroupShape groupShape = shapes.Group(shapesArr);
```
## See Also
* Class [GroupShape](../../groupshape/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../../shape/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
