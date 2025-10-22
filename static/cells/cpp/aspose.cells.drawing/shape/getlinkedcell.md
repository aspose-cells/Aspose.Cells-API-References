##Aspose::Cells::Drawing::Shape::GetLinkedCell method
'Aspose::Cells::Drawing::Shape::GetLinkedCell method. Gets or sets the worksheet range linked to the control''s value in C++.'
## Shape::GetLinkedCell() method
Gets or sets the worksheet range linked to the control's value.
```cpp
U16String Aspose::Cells::Drawing::Shape::GetLinkedCell()
```
## Examples
```cpp
if (shape.GetLinkedCell() == u"$B$6")
{
shape.SetLinkedCell(u"A1");
}
shape.UpdateSelectedValue();
```
## See Also
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## Shape::GetLinkedCell(bool, bool) method
Gets the range linked to the control's value.
```cpp
U16String Aspose::Cells::Drawing::Shape::GetLinkedCell(bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | bool | Whether the formula needs to be formatted as R1C1. |
| isLocal | bool | Whether the formula needs to be formatted by locale. |
## ReturnValue
The range linked to the control's value.
## Examples
```cpp
//You may get results like '$A$1'
U16String link = shape.GetLinkedCell(false, false);
```
## See Also
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
