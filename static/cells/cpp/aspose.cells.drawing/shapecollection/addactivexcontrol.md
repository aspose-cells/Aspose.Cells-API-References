##Aspose::Cells::Drawing::ShapeCollection::AddActiveXControl method
'Aspose::Cells::Drawing::ShapeCollection::AddActiveXControl method. Creates an Activex Control in C++.'
## ShapeCollection::AddActiveXControl method
Creates an Activex Control.
```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::AddActiveXControl(ControlType type, int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t width, int32_t height)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | ControlType | The type of the control. |
| topRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of [Shape](../../shape/) from its left row, in unit of pixel. |
| leftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of [Shape](../../shape/) from its left column, in unit of pixel. |
| height | int32_t | Represents the height of [Shape](../../shape/), in unit of pixel. |
| width | int32_t | Represents the width of [Shape](../../shape/), in unit of pixel. |
## ReturnValue
## Examples
```cpp
//add an ActiveX control
Shape activeXControl = shapes.AddActiveXControl(ControlType::CheckBox, 1, 0, 1, 0, 100, 50);
```
## See Also
* Class [Shape](../../shape/)
* Enum [ControlType](../../../aspose.cells.drawing.activexcontrols/controltype/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
