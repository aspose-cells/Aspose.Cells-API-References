##SignatureLine.Title
SignatureLine property. Gets or sets the title of singer
## SignatureLine.Title property
Gets or sets the title of singer.
```csharp
public string Title { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class SignatureLinePropertyTitleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a signature line and set its title
SignatureLine signatureLine = new SignatureLine();
signatureLine.Title = "Development Lead";
// Add the signature line to the worksheet's shapes with position parameters
worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);
// Output the title to demonstrate the property was set
Console.WriteLine("Signature Line Title: " + signatureLine.Title);
}
}
}
```
### See Also
* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
