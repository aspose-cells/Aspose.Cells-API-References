##Aspose::Cells::Drawing::ShapeCollection::AddLine method
'Aspose::Cells::Drawing::ShapeCollection::AddLine method. Adds a LineShape to the worksheet in C++.'
## ShapeCollection::AddLine method
Adds a [LineShape](../../lineshape/) to the worksheet.
```cpp
LineShape Aspose::Cells::Drawing::ShapeCollection::AddLine(int32_t upperLeftRow, int32_t top, int32_t upperLeftColumn, int32_t left, int32_t height, int32_t width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of [LineShape](../../lineshape/) from its left row, in unit of pixel. |
| upperLeftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of [LineShape](../../lineshape/) from its left column, in unit of pixel. |
| height | int32_t | Represents the height of [LineShape](../../lineshape/), in unit of pixel. |
| width | int32_t | Represents the width of [LineShape](../../lineshape/), in unit of pixel. |
## ReturnValue
A [LineShape](../../lineshape/) object.
## Examples
```cpp
// add a line object
LineShape lineShape = shapes.AddLine(1, 0, 1, 0, 100, 50);
```
## See Also
* Class [LineShape](../../lineshape/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
