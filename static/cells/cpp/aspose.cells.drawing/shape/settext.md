##Aspose::Cells::Drawing::Shape::SetText method
'Aspose::Cells::Drawing::Shape::SetText method. Gets and sets the text of this shape in C++.'
## Shape::SetText(const U16String\&) method
Gets and sets the text of this shape.
```cpp
void Aspose::Cells::Drawing::Shape::SetText(const U16String &value)
```
## Examples
```cpp
U16String val = u"This is a test.";
if (shape.GetText().IsNull())
shape.SetText(val);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## Shape::SetText(const char16_t*) method
Gets and sets the text of this shape.
```cpp
void Aspose::Cells::Drawing::Shape::SetText(const char16_t *value)
```
## Examples
```cpp
if (shape.GetText().IsNull())
shape.SetText(u"This is a test.");
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
