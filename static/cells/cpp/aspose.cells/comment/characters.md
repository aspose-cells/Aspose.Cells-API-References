##Aspose::Cells::Comment::Characters method
'Aspose::Cells::Comment::Characters method. Returns a Characters object that represents a range of characters within the comment text in C++.'
## Comment::Characters method
Returns a Characters object that represents a range of characters within the comment text.
```cpp
FontSetting Aspose::Cells::Comment::Characters(int32_t startIndex, int32_t length)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int32_t | The index of the start of the character. |
| length | int32_t | The number of characters. |
## ReturnValue
Characters object.
## Examples
```cpp
FontSetting fontSetting = comment1.Characters(0, 4);
```
## See Also
* Class [FontSetting](../../fontsetting/)
* Class [Vector](../../vector/)
* Class [Comment](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
