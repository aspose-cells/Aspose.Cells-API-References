##Aspose::Cells::Drawing::SignatureLine::SetInstructions method
'Aspose::Cells::Drawing::SignatureLine::SetInstructions method. Gets or sets the text shown to user at signing time in C++.'
## SignatureLine::SetInstructions(const U16String\&) method
Gets or sets the text shown to user at signing time.
```cpp
void Aspose::Cells::Drawing::SignatureLine::SetInstructions(const U16String &value)
```
## Examples
```cpp
// Create signature line object
U16String val = u"Just do it.";
SignatureLine s6;
if (s6.GetInstructions().IsNull() || s6.GetInstructions().IsEmpty())
{
s6.SetInstructions(val);
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [SignatureLine](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## SignatureLine::SetInstructions(const char16_t*) method
Gets or sets the text shown to user at signing time.
```cpp
void Aspose::Cells::Drawing::SignatureLine::SetInstructions(const char16_t *value)
```
## Examples
```cpp
// Create signature line object
SignatureLine s6;
if (s6.GetInstructions().IsNull() || s6.GetInstructions().IsEmpty())
{
s6.SetInstructions(u"Just do it.");
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [SignatureLine](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
