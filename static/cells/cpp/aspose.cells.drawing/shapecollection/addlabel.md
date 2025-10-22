##Aspose::Cells::Drawing::ShapeCollection::AddLabel method
'Aspose::Cells::Drawing::ShapeCollection::AddLabel method. Adds a Label to the worksheet in C++.'
## ShapeCollection::AddLabel method
Adds a [Label](../../label/) to the worksheet.
```cpp
Label Aspose::Cells::Drawing::ShapeCollection::AddLabel(int32_t upperLeftRow, int32_t top, int32_t upperLeftColumn, int32_t left, int32_t height, int32_t width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of [Label](../../label/) from its left row, in unit of pixel. |
| upperLeftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of [Label](../../label/) from its left column, in unit of pixel. |
| height | int32_t | Represents the height of [Label](../../label/), in unit of pixel. |
| width | int32_t | Represents the width of [Label](../../label/), in unit of pixel. |
## ReturnValue
A [Label](../../label/) object.
## Examples
```cpp
//add a label
Label label = shapes.AddLabel(1, 0, 1, 0, 100, 50);
```
## See Also
* Class [Label](../../label/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
