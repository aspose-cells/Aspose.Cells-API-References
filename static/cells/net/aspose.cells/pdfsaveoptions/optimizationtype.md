##PdfSaveOptions.OptimizationType
PdfSaveOptions property. Gets and sets pdf optimization type
## PdfSaveOptions.OptimizationType property
Gets and sets pdf optimization type.
```csharp
public PdfOptimizationType OptimizationType { get; set; }
```
### Remarks
Default value is Standard
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class PdfSaveOptionsPropertyOptimizationTypeDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Optimization Example");
// Create PDF save options
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
// Demonstrate OptimizationType property
pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;
// Save the workbook with optimization settings
workbook.Save("OptimizedPdf.pdf", pdfSaveOptions);
}
}
}
```
### See Also
* enum [PdfOptimizationType](../../../aspose.cells.rendering/pdfoptimizationtype/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
