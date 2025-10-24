##PdfSaveOptions.CalculateFormula
PdfSaveOptions property. Indicates whether to calculate formulas before saving pdf file
## PdfSaveOptions.CalculateFormula property
Indicates whether to calculate formulas before saving pdf file.
```csharp
public bool CalculateFormula { get; set; }
```
### Remarks
The default value is false.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PdfSaveOptionsPropertyCalculateFormulaDemo
{
public static void Run()
{
// Create a workbook with sample data and formulas
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set values and formulas
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";
// Create PDF save options with formula calculation
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.CalculateFormula = true;
// Save to memory stream
using (MemoryStream stream = new MemoryStream())
{
workbook.Save(stream, pdfSaveOptions);
// Reset stream position and verify content
stream.Position = 0;
using (StreamReader reader = new StreamReader(stream))
{
string content = reader.ReadToEnd();
Console.WriteLine("PDF contains formula results: " + content.Contains("30"));
}
}
}
}
}
```
### See Also
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
