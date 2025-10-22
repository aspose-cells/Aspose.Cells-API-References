##Picture.SignatureLine
Picture property. Gets and sets the signature line
## Picture.SignatureLine property
Gets and sets the signature line
```csharp
public SignatureLine SignatureLine { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PicturePropertySignatureLineDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int imgIndex = worksheet.Pictures.Add(1, 1, (string)null);
Picture pic = worksheet.Pictures[imgIndex];
SignatureLine signatureLine = new SignatureLine();
signatureLine.Signer = "Simon";
signatureLine.Title = "Development";
signatureLine.Email = "simon@aspose.com";
pic.SignatureLine = signatureLine;
workbook.Save("result.xlsx");
}
}
}
```
### See Also
* class [SignatureLine](../../signatureline/)
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
