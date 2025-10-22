##Aspose::Cells::Drawing::SignatureLine::GetSigner method
'Aspose::Cells::Drawing::SignatureLine::GetSigner method. Gets or sets the signer in C++.'
## SignatureLine::GetSigner method
Gets or sets the signer.
```cpp
U16String Aspose::Cells::Drawing::SignatureLine::GetSigner()
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
* Class [U16String](../../../aspose.cells/u16string/)
* Class [SignatureLine](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
