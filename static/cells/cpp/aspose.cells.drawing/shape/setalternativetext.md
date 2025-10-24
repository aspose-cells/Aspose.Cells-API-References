##Aspose::Cells::Drawing::Shape::SetAlternativeText method
'Aspose::Cells::Drawing::Shape::SetAlternativeText method. Returns or sets the descriptive (alternative) text string of the Shape object in C++.'
## Shape::SetAlternativeText(const U16String\&) method
Returns or sets the descriptive (alternative) text string of the [Shape](../) object.
```cpp
void Aspose::Cells::Drawing::Shape::SetAlternativeText(const U16String &value)
```
## Examples
```cpp
U16String txt = u"a rectangle";
if (shape.GetAlternativeText() == u"rectangle")
{
shape.SetAlternativeText(txt);
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## Shape::SetAlternativeText(const char16_t*) method
Returns or sets the descriptive (alternative) text string of the [Shape](../) object.
```cpp
void Aspose::Cells::Drawing::Shape::SetAlternativeText(const char16_t *value)
```
## Examples
```cpp
if (shape.GetAlternativeText() == u"rectangle")
{
shape.SetAlternativeText(u"a rectangle");
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
