##Aspose::Cells::Drawing::Shape::SetLinkedCell method
'Aspose::Cells::Drawing::Shape::SetLinkedCell method. Gets or sets the worksheet range linked to the control''s value in C++.'
## Shape::SetLinkedCell(const U16String\&) method
Gets or sets the worksheet range linked to the control's value.
```cpp
void Aspose::Cells::Drawing::Shape::SetLinkedCell(const U16String &value)
```
## Examples
```cpp
U16String val = u"A1";
if (shape.GetLinkedCell() == u"$B$6")
shape.SetLinkedCell(val);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## Shape::SetLinkedCell(const char16_t*) method
Gets or sets the worksheet range linked to the control's value.
```cpp
void Aspose::Cells::Drawing::Shape::SetLinkedCell(const char16_t *value)
```
## Examples
```cpp
if (shape.GetLinkedCell() == u"$B$6")
shape.SetLinkedCell(u"A1");
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## Shape::SetLinkedCell(const U16String\&, bool, bool) method
Sets the range linked to the control's value.
```cpp
void Aspose::Cells::Drawing::Shape::SetLinkedCell(const U16String &formula, bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const U16String\& | The range linked to the control's value. |
| isR1C1 | bool | Whether the formula needs to be formatted as R1C1. |
| isLocal | bool | Whether the formula needs to be formatted by locale. |
## Examples
```cpp
//After executing the code below, a ScrollBar object is created in the generated file. As you drag the slider, the value is displayed in cell A12.
//ActiveX Controls
//Aspose.Cells.Drawing.Shape scrollBar = book.GetWorksheets().Get(0).GetShapes().AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType::ScrollBar,2, 0, 2, 0, 30, 130);
//Form Controls
Shape scrollBar = book.GetWorksheets().Get(0).GetShapes().AddScrollBar(2, 0, 2, 0, 130, 30);
//Sets the range linked to the control's value.
U16String val = u"$A$12";
scrollBar.SetLinkedCell(val, false, true);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## Shape::SetLinkedCell(const char16_t*, bool, bool) method
Sets the range linked to the control's value.
```cpp
void Aspose::Cells::Drawing::Shape::SetLinkedCell(const char16_t *formula, bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const char16_t* | The range linked to the control's value. |
| isR1C1 | bool | Whether the formula needs to be formatted as R1C1. |
| isLocal | bool | Whether the formula needs to be formatted by locale. |
## Examples
```cpp
//After executing the code below, a ScrollBar object is created in the generated file. As you drag the slider, the value is displayed in cell A12.
//ActiveX Controls
//Aspose.Cells.Drawing.Shape scrollBar = book.GetWorksheets().Get(0).GetShapes().AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType::ScrollBar,2, 0, 2, 0, 30, 130);
//Form Controls
Shape scrollBar = book.GetWorksheets().Get(0).GetShapes().AddScrollBar(2, 0, 2, 0, 130, 30);
//Sets the range linked to the control's value.
scrollBar.SetLinkedCell(u"$A$12", false, true);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
