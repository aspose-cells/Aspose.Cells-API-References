##Aspose::Cells::Drawing::Shape::GetInputRange method
'Aspose::Cells::Drawing::Shape::GetInputRange method. Gets or sets the worksheet range used to fill the specified combo box in C++.'
## Shape::GetInputRange() method
Gets or sets the worksheet range used to fill the specified combo box.
```cpp
U16String Aspose::Cells::Drawing::Shape::GetInputRange()
```
## Examples
```cpp
if (shape.GetInputRange() == u"$B$6:$B10")
shape.SetInputRange(u"$A$1:$A$5");
```
## See Also
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## Shape::GetInputRange(bool, bool) method
Gets the range used to fill the control.
```cpp
U16String Aspose::Cells::Drawing::Shape::GetInputRange(bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | bool | Whether the formula needs to be formatted as R1C1. |
| isLocal | bool | Whether the formula needs to be formatted by locale. |
## ReturnValue
The range used to fill the control.
## Examples
```cpp
U16String range = shape.GetInputRange(false, true);
//If successful, a value like "$A$1:$A$3" will be returned
```
## See Also
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
