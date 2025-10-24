##Aspose::Cells::Drawing::Shape::SetInputRange method
'Aspose::Cells::Drawing::Shape::SetInputRange method. Gets or sets the worksheet range used to fill the specified combo box in C++.'
## Shape::SetInputRange(const U16String\&) method
Gets or sets the worksheet range used to fill the specified combo box.
```cpp
void Aspose::Cells::Drawing::Shape::SetInputRange(const U16String &value)
```
## Examples
```cpp
U16String range = u"$A$1:$A$5";
if (shape.GetInputRange() == u"$B$6:$B10")
shape.SetInputRange(range);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## Shape::SetInputRange(const char16_t*) method
Gets or sets the worksheet range used to fill the specified combo box.
```cpp
void Aspose::Cells::Drawing::Shape::SetInputRange(const char16_t *value)
```
## Examples
```cpp
if (shape.GetInputRange() == u"$B$6:$B10")
shape.SetInputRange(u"$A$1:$A$5");
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## Shape::SetInputRange(const U16String\&, bool, bool) method
Sets the range used to fill the control.
```cpp
void Aspose::Cells::Drawing::Shape::SetInputRange(const U16String &formula, bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const U16String\& | The range used to fill the control. |
| isR1C1 | bool | Whether the formula needs to be formatted as R1C1. |
| isLocal | bool | Whether the formula needs to be formatted by locale. |
## Examples
```cpp
//After executing the code below, a ListBox object is created in the generated file. When the selected option is clicked, the selected value is displayed in cell A12.
for (int i = 0; i < 10; ++i)
{
Cell cell = book.GetWorksheets().Get(0).GetCells().Get(i, 0);
cell.PutValue(i + 1);
}
//Create a ListBox object
//ActiveX Controls
//Aspose.Cells.Drawing.Shape listBox = book.GetWorksheets().Get(0).GetShapes().AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType::ListBox,2, 0, 2, 0, 130, 130);
//Form Controls
Shape listBox = book.GetWorksheets().Get(0).GetShapes().AddListBox(2, 0, 2, 0, 130, 130);
//Sets the range used to fill the control.
U16String val = u"$A$1:$A$6";
listBox.SetInputRange(val, false, false);
//Sets the range linked to the control's value.
listBox.SetLinkedCell(u"$A$12", false, true);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## Shape::SetInputRange(const char16_t*, bool, bool) method
Sets the range used to fill the control.
```cpp
void Aspose::Cells::Drawing::Shape::SetInputRange(const char16_t *formula, bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const char16_t* | The range used to fill the control. |
| isR1C1 | bool | Whether the formula needs to be formatted as R1C1. |
| isLocal | bool | Whether the formula needs to be formatted by locale. |
## Examples
```cpp
//After executing the code below, a ListBox object is created in the generated file. When the selected option is clicked, the selected value is displayed in cell A12.
for (int i = 0; i < 10; ++i)
{
Cell cell = book.GetWorksheets().Get(0).GetCells().Get(i, 0);
cell.PutValue(i + 1);
}
//Create a ListBox object
//ActiveX Controls
//Aspose.Cells.Drawing.Shape listBox = book.GetWorksheets().Get(0).GetShapes().AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType::ListBox,2, 0, 2, 0, 130, 130);
//Form Controls
Shape listBox = book.GetWorksheets().Get(0).GetShapes().AddListBox(2, 0, 2, 0, 130, 130);
//Sets the range used to fill the control.
listBox.SetInputRange(u"$A$1:$A$6", false, false);
//Sets the range linked to the control's value.
listBox.SetLinkedCell(u"$A$12", false, true);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
