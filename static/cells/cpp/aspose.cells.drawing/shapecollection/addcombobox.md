##Aspose::Cells::Drawing::ShapeCollection::AddComboBox method
'Aspose::Cells::Drawing::ShapeCollection::AddComboBox method. Adds a ComboBox to the worksheet in C++.'
## ShapeCollection::AddComboBox method
Adds a [ComboBox](../../combobox/) to the worksheet.
```cpp
ComboBox Aspose::Cells::Drawing::ShapeCollection::AddComboBox(int32_t upperLeftRow, int32_t top, int32_t upperLeftColumn, int32_t left, int32_t height, int32_t width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of [ComboBox](../../combobox/) from its left row, in unit of pixel. |
| upperLeftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of [ComboBox](../../combobox/) from its left column, in unit of pixel. |
| height | int32_t | Represents the height of [ComboBox](../../combobox/), in unit of pixel. |
| width | int32_t | Represents the width of [ComboBox](../../combobox/), in unit of pixel. |
## ReturnValue
A [ComboBox](../../combobox/) object.
## Examples
```cpp
//add a combo box
ComboBox comboBox = shapes.AddComboBox(1, 0, 1, 0, 100, 50);
```
## See Also
* Class [ComboBox](../../combobox/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
