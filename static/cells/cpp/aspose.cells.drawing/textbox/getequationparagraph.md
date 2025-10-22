##Aspose::Cells::Drawing::TextBox::GetEquationParagraph method
'Aspose::Cells::Drawing::TextBox::GetEquationParagraph method. Get the specified math paragraph from the TextBody property of the TextBox object. Notice: (1) Returns NULL when the index is out of bounds or not found. (2) Also returns NULL if the specified index position is not a math paragraph in C++.'
## TextBox::GetEquationParagraph(int32_t) method
Get the specified math paragraph from the TextBody property of the [TextBox](../) object. Notice: (1) Returns NULL when the index is out of bounds or not found. (2) Also returns NULL if the specified index position is not a math paragraph.
```cpp
EquationNode Aspose::Cells::Drawing::TextBox::GetEquationParagraph(int32_t index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | int32_t | The position index of the math paragraph, starting from 0. |
## ReturnValue
Returns the math paragraph specified by index.
## See Also
* Class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [TextBox](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## TextBox::GetEquationParagraph() method
Gets the first math paragraph from the TextBody property of the [TextBox](../) object.
```cpp
EquationNode Aspose::Cells::Drawing::TextBox::GetEquationParagraph()
```
## ReturnValue
If there has math paragraph, returns the first one, otherwise returns null.
## See Also
* Class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* Class [TextBox](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
