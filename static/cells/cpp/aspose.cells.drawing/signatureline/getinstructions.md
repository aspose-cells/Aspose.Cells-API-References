##Aspose::Cells::Drawing::SignatureLine::GetInstructions method
'Aspose::Cells::Drawing::SignatureLine::GetInstructions method. Gets or sets the text shown to user at signing time in C++.'
## SignatureLine::GetInstructions method
Gets or sets the text shown to user at signing time.
```cpp
U16String Aspose::Cells::Drawing::SignatureLine::GetInstructions()
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
* Class [U16String](../../../aspose.cells/u16string/)
* Class [SignatureLine](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
