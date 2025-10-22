##Aspose::Cells::Drawing::Shape::SetMacroName method
'Aspose::Cells::Drawing::Shape::SetMacroName method. Gets and sets the name of macro in C++.'
## Shape::SetMacroName(const U16String\&) method
Gets and sets the name of macro.
```cpp
void Aspose::Cells::Drawing::Shape::SetMacroName(const U16String &value)
```
## Examples
```cpp
U16String val = u"DoWork()";
//Sets the name of macro.
if (shape.GetMacroName().IsNull())
{
shape.SetMacroName(val);
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## Shape::SetMacroName(const char16_t*) method
Gets and sets the name of macro.
```cpp
void Aspose::Cells::Drawing::Shape::SetMacroName(const char16_t *value)
```
## Examples
```cpp
//Sets the name of macro.
if (shape.GetMacroName().IsNull())
{
shape.SetMacroName(u"DoWork()");
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
