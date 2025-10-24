##Aspose::Cells::Drawing::ShapeCollection::AddSpinner method
'Aspose::Cells::Drawing::ShapeCollection::AddSpinner method. Adds a Spinner to the worksheet in C++.'
## ShapeCollection::AddSpinner method
Adds a [Spinner](../../spinner/) to the worksheet.
```cpp
Spinner Aspose::Cells::Drawing::ShapeCollection::AddSpinner(int32_t upperLeftRow, int32_t top, int32_t upperLeftColumn, int32_t left, int32_t height, int32_t width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of [Spinner](../../spinner/) from its left row, in unit of pixel. |
| upperLeftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of [Spinner](../../spinner/) from its left column, in unit of pixel. |
| height | int32_t | Represents the height of [Spinner](../../spinner/), in unit of pixel. |
| width | int32_t | Represents the width of [Spinner](../../spinner/), in unit of pixel. |
## ReturnValue
A [Spinner](../../spinner/) object.
## Examples
```cpp
//add a spinner
Spinner spinner = shapes.AddSpinner(1, 0, 1, 0, 100, 50);
```
## See Also
* Class [Spinner](../../spinner/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
