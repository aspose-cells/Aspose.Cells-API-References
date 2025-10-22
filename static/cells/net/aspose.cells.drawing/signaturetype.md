##Enum SignatureType
Aspose.Cells.Drawing.SignatureType enum. Specifies the signature type
## SignatureType enumeration
Specifies the signature type.
```csharp
public enum SignatureType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Default | `0` | The default value , the corresponding ProviderId value is fixed to {0000000000-0000-0000-0000-0000000000}. |
| Stamp | `1` | The corresponding ProviderId value is usually {000CD6A4-0000-0000-C000-000000000046}. |
| Custom | `3` | The corresponding ProviderId value usually needs to be set by the user. it should be obtained from the documentation shipped with the provider. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class DrawingClassSignatureTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add signature lines with different types
Picture stampPicture = worksheet.Shapes.AddSignatureLine(3, 1, new SignatureLine());
stampPicture.SignatureLine.SignatureLineType = SignatureType.Stamp;
Picture customPicture = worksheet.Shapes.AddSignatureLine(8, 1, new SignatureLine());
customPicture.SignatureLine.SignatureLineType = SignatureType.Custom;
customPicture.SignatureLine.ProviderId = new Guid("12345678-ABCD-4321-5678-9876543210AB");
// Save the workbook with signature configurations
workbook.Save("SignatureTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
