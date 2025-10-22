##Aspose::Cells::Drawing::ShapeCollection::AddRadioButton method
'Aspose::Cells::Drawing::ShapeCollection::AddRadioButton method. Adds a RadioButton to the worksheet in C++.'
## ShapeCollection::AddRadioButton method
Adds a [RadioButton](../../radiobutton/) to the worksheet.
```cpp
RadioButton Aspose::Cells::Drawing::ShapeCollection::AddRadioButton(int32_t upperLeftRow, int32_t top, int32_t upperLeftColumn, int32_t left, int32_t height, int32_t width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of [RadioButton](../../radiobutton/) from its left row, in unit of pixel. |
| upperLeftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of [RadioButton](../../radiobutton/) from its left column, in unit of pixel. |
| height | int32_t | Represents the height of [RadioButton](../../radiobutton/), in unit of pixel. |
| width | int32_t | Represents the width of [RadioButton](../../radiobutton/), in unit of pixel. |
## ReturnValue
A [RadioButton](../../radiobutton/) object.
## Examples
```cpp
//add a radio button
RadioButton radioButton = shapes.AddRadioButton(1, 0, 1, 0, 100, 50);
```
## See Also
* Class [RadioButton](../../radiobutton/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
