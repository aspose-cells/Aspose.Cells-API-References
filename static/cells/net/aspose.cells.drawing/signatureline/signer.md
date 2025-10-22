##SignatureLine.Signer
SignatureLine property. Gets or sets the signer
## SignatureLine.Signer property
Gets or sets the signer.
```csharp
public string Signer { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class SignatureLinePropertySignerDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a signature line and set its properties
SignatureLine signatureLine = new SignatureLine();
signatureLine.Signer = "John Doe";
signatureLine.Title = "Software Developer";
signatureLine.Email = "john.doe@example.com";
// Add the signature line to the worksheet at row 1, column 1
worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);
// Save the workbook
workbook.Save("SignatureLineDemo.xlsx");
}
}
}
```
### See Also
* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
