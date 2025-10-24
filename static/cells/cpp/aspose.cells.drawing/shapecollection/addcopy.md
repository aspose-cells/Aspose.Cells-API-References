##Aspose::Cells::Drawing::ShapeCollection::AddCopy method
'Aspose::Cells::Drawing::ShapeCollection::AddCopy method. Adds and copy a shape to the worksheet in C++.'
## ShapeCollection::AddCopy method
Adds and copy a shape to the worksheet.
```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::AddCopy(const Shape &sourceShape, int32_t topRow, int32_t top, int32_t leftColumn, int32_t left)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceShape | const Shape\& | Source shape. |
| topRow | int32_t | The top row index. |
| top | int32_t | Represents the vertical offset from its top row, in unit of pixel. |
| leftColumn | int32_t | The left column index. |
| left | int32_t | Represents the horizontal offset from its left column, in unit of pixel. |
## ReturnValue
The new [Shape](../../shape/) object.
## Examples
```cpp
//add a shape
RectangleShape rectangle = shapes.AddRectangle(2, 0, 2, 0, 130, 130);
//Adds and copies a shape.
shapes.AddCopy(rectangle, 7, 0, 7, 0);
```
## See Also
* Class [Shape](../../shape/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
