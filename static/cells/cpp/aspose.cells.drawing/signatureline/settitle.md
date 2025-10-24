##Aspose::Cells::Drawing::SignatureLine::SetTitle method
'Aspose::Cells::Drawing::SignatureLine::SetTitle method. Gets or sets the title of singer in C++.'
## SignatureLine::SetTitle(const U16String\&) method
Gets or sets the title of singer.
```cpp
void Aspose::Cells::Drawing::SignatureLine::SetTitle(const U16String &value)
```
## Examples
```cpp
// Create signature line object
U16String val = u"Development Lead";
SignatureLine s4;
if (s4.GetTitle().IsNull() || s4.GetTitle().IsEmpty())
{
s4.SetTitle(val);
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [SignatureLine](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## SignatureLine::SetTitle(const char16_t*) method
Gets or sets the title of singer.
```cpp
void Aspose::Cells::Drawing::SignatureLine::SetTitle(const char16_t *value)
```
## Examples
```cpp
// Create signature line object
SignatureLine s4;
if (s4.GetTitle().IsNull() || s4.GetTitle().IsEmpty())
{
s4.SetTitle(u"Development Lead");
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [SignatureLine](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
