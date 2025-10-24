##PdfSaveOptions.PdfSaveOptions
PdfSaveOptions constructor. Creates the options for saving pdf file
## PdfSaveOptions constructor
Creates the options for saving pdf file.
```csharp
public PdfSaveOptions()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class PdfSaveOptionsMethodCtorDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Hello World!");
// Demonstrate PdfSaveOptions constructor
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.Compliance = PdfCompliance.PdfA1b;
// Save the workbook with PDF options
workbook.Save("output.pdf", pdfSaveOptions);
Console.WriteLine("PDF saved successfully with PdfA1b compliance.");
}
}
}
```
### See Also
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
