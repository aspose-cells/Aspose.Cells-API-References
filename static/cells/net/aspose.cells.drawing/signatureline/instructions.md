##SignatureLine.Instructions
SignatureLine property. Gets or sets the text shown to user at signing time
## SignatureLine.Instructions property
Gets or sets the text shown to user at signing time.
```csharp
public string Instructions { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class SignatureLinePropertyInstructionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a signature line object
SignatureLine signatureLine = new SignatureLine();
signatureLine.Instructions = "Please sign here after reviewing the document.";
// Add the signature line to the worksheet at position (1,1)
worksheet.Shapes.AddSignatureLine(1, 1, signatureLine);
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
