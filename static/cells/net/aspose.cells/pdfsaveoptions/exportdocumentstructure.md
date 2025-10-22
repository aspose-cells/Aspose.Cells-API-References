##PdfSaveOptions.ExportDocumentStructure
PdfSaveOptions property. Indicates whether to export document structure
## PdfSaveOptions.ExportDocumentStructure property
Indicates whether to export document structure.
```csharp
public bool ExportDocumentStructure { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PdfSaveOptionsPropertyExportDocumentStructureDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Create PDF save options
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
// Set ExportDocumentStructure to true to retain document structure
pdfSaveOptions.ExportDocumentStructure = true;
// Calculate formulas before saving
workbook.CalculateFormula();
// Save the workbook to PDF with the specified options
workbook.Save("output.pdf", pdfSaveOptions);
Console.WriteLine("PDF saved with document structure exported.");
}
}
}
```
### See Also
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
