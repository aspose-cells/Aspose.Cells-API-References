##Aspose::Cells::Drawing::ShapeCollection::AddSignatureLine method
'Aspose::Cells::Drawing::ShapeCollection::AddSignatureLine method. Adds a Signature Line to the worksheet in C++.'
## ShapeCollection::AddSignatureLine method
Adds a Signature [Line](../../line/) to the worksheet.
```cpp
Aspose::Cells::Drawing::Picture Aspose::Cells::Drawing::ShapeCollection::AddSignatureLine(int32_t upperLeftRow, int32_t upperLeftColumn, const SignatureLine &signatureLine)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int32_t | Upper left row index. |
| upperLeftColumn | int32_t | Upper left column index. |
| signatureLine | const SignatureLine\& | Represents a signature line object. |
## ReturnValue
## Examples
```cpp
SignatureLine wSignatureLine;
wSignatureLine.SetAllowComments(true);
wSignatureLine.SetEmail(u"example@example.com");
wSignatureLine.SetInstructions(u"Sign to confirm the excel content.");
wSignatureLine.SetIsLine(true);
wSignatureLine.SetShowSignedDate(true);
wSignatureLine.SetSigner(u"User");
wSignatureLine.SetTitle(u"tester");
//wSignatureLine.SignatureLineType = SignatureType.Stamp;
Picture signatureLine1 = shapes.AddSignatureLine(0, 0, wSignatureLine);
```
## See Also
* Class [Picture](../../picture/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [SignatureLine](../../signatureline/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
