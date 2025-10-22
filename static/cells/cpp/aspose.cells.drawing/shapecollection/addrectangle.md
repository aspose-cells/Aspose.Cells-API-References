##Aspose::Cells::Drawing::ShapeCollection::AddRectangle method
'Aspose::Cells::Drawing::ShapeCollection::AddRectangle method. Adds a RectangleShape to the worksheet in C++.'
## ShapeCollection::AddRectangle method
Adds a [RectangleShape](../../rectangleshape/) to the worksheet.
```cpp
RectangleShape Aspose::Cells::Drawing::ShapeCollection::AddRectangle(int32_t upperLeftRow, int32_t top, int32_t upperLeftColumn, int32_t left, int32_t height, int32_t width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of [RectangleShape](../../rectangleshape/) from its left row, in unit of pixel. |
| upperLeftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of [RectangleShape](../../rectangleshape/) from its left column, in unit of pixel. |
| height | int32_t | Represents the height of [RectangleShape](../../rectangleshape/), in unit of pixel. |
| width | int32_t | Represents the width of [RectangleShape](../../rectangleshape/), in unit of pixel. |
## ReturnValue
A [RectangleShape](../../rectangleshape/) object.
## Examples
```cpp
// add a rectangle
RectangleShape rectangleShape = shapes.AddRectangle(2, 0, 2, 0, 130, 130);
```
## See Also
* Class [RectangleShape](../../rectangleshape/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
