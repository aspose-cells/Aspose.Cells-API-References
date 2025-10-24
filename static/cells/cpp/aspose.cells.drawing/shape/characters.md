##Aspose::Cells::Drawing::Shape::Characters method
'Aspose::Cells::Drawing::Shape::Characters method. Returns a Characters object that represents a range of characters within the text in C++.'
## Shape::Characters method
Returns a Characters object that represents a range of characters within the text.
```cpp
FontSetting Aspose::Cells::Drawing::Shape::Characters(int32_t startIndex, int32_t length)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int32_t | The index of the start of the character. |
| length | int32_t | The number of characters. |
## ReturnValue
Characters object.
## Remarks
This method only works on shape with title.
## Examples
```cpp
FontSetting fontSetting = shape.Characters(0, 4);
```
## See Also
* Class [FontSetting](../../../aspose.cells/fontsetting/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
