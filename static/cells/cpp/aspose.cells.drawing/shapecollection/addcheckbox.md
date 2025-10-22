##Aspose::Cells::Drawing::ShapeCollection::AddCheckBox method
'Aspose::Cells::Drawing::ShapeCollection::AddCheckBox method. Adds a checkbox to the worksheet in C++.'
## ShapeCollection::AddCheckBox method
Adds a checkbox to the worksheet.
```cpp
CheckBox Aspose::Cells::Drawing::ShapeCollection::AddCheckBox(int32_t upperLeftRow, int32_t top, int32_t upperLeftColumn, int32_t left, int32_t height, int32_t width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of checkbox from its top row, in unit of pixel. |
| upperLeftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of textbox from its left column, in unit of pixel. |
| height | int32_t | Height of textbox, in unit of pixel. |
| width | int32_t | Width of textbox, in unit of pixel. |
## ReturnValue
The new [CheckBox](../../checkbox/) object index.
## Examples
```cpp
//add a CheckBox
CheckBox checkBox = shapes.AddCheckBox(1, 0, 1, 0, 100, 50);
```
## See Also
* Class [CheckBox](../../checkbox/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
