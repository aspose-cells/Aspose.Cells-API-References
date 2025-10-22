##SignatureLine.Id
SignatureLine property. Gets or sets identifier for this signature line
## SignatureLine.Id property
Gets or sets identifier for this signature line.
```csharp
public Guid Id { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class SignatureLinePropertyIdDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a signature line object
SignatureLine signatureLine = new SignatureLine();
Guid signatureId = Guid.NewGuid();
signatureLine.Id = signatureId;
// Add the signature line to the worksheet at position (1,1)
worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);
// Display the ID of the signature line
Console.WriteLine("Signature Line ID: " + signatureLine.Id);
}
}
}
```
### See Also
* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
