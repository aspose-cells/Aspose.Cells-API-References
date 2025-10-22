##Aspose::Cells::Drawing::ShapeCollection::AddTextBox method
'Aspose::Cells::Drawing::ShapeCollection::AddTextBox method. Adds a text box to the worksheet in C++.'
## ShapeCollection::AddTextBox method
Adds a text box to the worksheet.
```cpp
TextBox Aspose::Cells::Drawing::ShapeCollection::AddTextBox(int32_t upperLeftRow, int32_t top, int32_t upperLeftColumn, int32_t left, int32_t height, int32_t width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of textbox from its top row, in unit of pixel. |
| upperLeftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of textbox from its left column, in unit of pixel. |
| height | int32_t | Represents the height of textbox, in unit of pixel. |
| width | int32_t | Represents the width of textbox, in unit of pixel. |
## ReturnValue
A [TextBox](../../textbox/) object.
## Examples
```cpp
//add a TextBox
TextBox textBox = shapes.AddTextBox(1, 0, 1, 0, 100, 50);
```
## See Also
* Class [TextBox](../../textbox/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
