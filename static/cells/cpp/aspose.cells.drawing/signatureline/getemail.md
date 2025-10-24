##Aspose::Cells::Drawing::SignatureLine::GetEmail method
'Aspose::Cells::Drawing::SignatureLine::GetEmail method. Gets or sets the email of singer in C++.'
## SignatureLine::GetEmail method
Gets or sets the email of singer.
```cpp
U16String Aspose::Cells::Drawing::SignatureLine::GetEmail()
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
* Class [U16String](../../../aspose.cells/u16string/)
* Class [SignatureLine](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
