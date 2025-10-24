##Aspose::Cells::Drawing::SignatureLine::SetSigner method
'Aspose::Cells::Drawing::SignatureLine::SetSigner method. Gets or sets the signer in C++.'
## SignatureLine::SetSigner(const U16String\&) method
Gets or sets the signer.
```cpp
void Aspose::Cells::Drawing::SignatureLine::SetSigner(const U16String &value)
```
## Examples
```cpp
// Create signature line object
U16String val = u"Mr xxx";
SignatureLine s3;
if (s3.GetSigner().IsNull() || s3.GetSigner().IsEmpty())
{
s3.SetSigner(val);
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [SignatureLine](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## SignatureLine::SetSigner(const char16_t*) method
Gets or sets the signer.
```cpp
void Aspose::Cells::Drawing::SignatureLine::SetSigner(const char16_t *value)
```
## Examples
```cpp
// Create signature line object
SignatureLine s3;
if (s3.GetSigner().IsNull() || s3.GetSigner().IsEmpty())
{
s3.SetSigner(u"Mr xxx");
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [SignatureLine](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
