##Aspose::Cells::Drawing::Shape::SetTitle method
'Aspose::Cells::Drawing::Shape::SetTitle method. Specifies the title (caption) of the current shape object in C++.'
## Shape::SetTitle(const U16String\&) method
Specifies the title (caption) of the current shape object.
```cpp
void Aspose::Cells::Drawing::Shape::SetTitle(const U16String &value)
```
## Examples
```cpp
U16String title = u"title1";
if (shape.GetTitle() == u"title")
{
shape.SetTitle(title);
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## Shape::SetTitle(const char16_t*) method
Specifies the title (caption) of the current shape object.
```cpp
void Aspose::Cells::Drawing::Shape::SetTitle(const char16_t *value)
```
## Examples
```cpp
if (shape.GetTitle() == u"title")
{
shape.SetTitle(u"title1");
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
