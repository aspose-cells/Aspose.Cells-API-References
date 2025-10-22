##Aspose::Cells::Drawing::SignatureLine::SetEmail method
'Aspose::Cells::Drawing::SignatureLine::SetEmail method. Gets or sets the email of singer in C++.'
## SignatureLine::SetEmail(const U16String\&) method
Gets or sets the email of singer.
```cpp
void Aspose::Cells::Drawing::SignatureLine::SetEmail(const U16String &value)
```
## Examples
```cpp
// Create signature line object
U16String val = u"Simon.Zhao@aspose.com";
SignatureLine s5;
if (s5.GetEmail().IsNull() || s5.GetEmail().IsEmpty())
{
s5.SetEmail(val);
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [SignatureLine](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## SignatureLine::SetEmail(const char16_t*) method
Gets or sets the email of singer.
```cpp
void Aspose::Cells::Drawing::SignatureLine::SetEmail(const char16_t *value)
```
## Examples
```cpp
// Create signature line object
SignatureLine s5;
if (s5.GetEmail().IsNull() || s5.GetEmail().IsEmpty())
{
s5.SetEmail(u"Simon.Zhao@aspose.com");
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [SignatureLine](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
