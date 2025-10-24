##Aspose::Cells::Drawing::Shape::IsLocked method
'Aspose::Cells::Drawing::Shape::IsLocked method. True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected in C++.'
## Shape::IsLocked method
True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected.
```cpp
bool Aspose::Cells::Drawing::Shape::IsLocked()
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
