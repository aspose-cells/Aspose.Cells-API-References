##Aspose::Cells::Drawing::Shape::SetIsLocked method
'Aspose::Cells::Drawing::Shape::SetIsLocked method. True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected in C++.'
## Shape::SetIsLocked method
True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected.
```cpp
void Aspose::Cells::Drawing::Shape::SetIsLocked(bool value)
```
## Examples
```cpp
//Sets the specified shape to unlocked state
if (shape.GetWorksheet().IsProtected() && shape.IsLocked())
{
shape.SetIsLocked(false);
}
//Sets the specified shape to a locked state
if (shape.GetWorksheet().IsProtected() && !shape.IsLocked())
{
shape.SetIsLocked(true);
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
