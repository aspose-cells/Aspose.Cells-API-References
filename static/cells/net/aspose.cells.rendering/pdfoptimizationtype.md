##Enum PdfOptimizationType
Aspose.Cells.Rendering.PdfOptimizationType enum. Specifies a type of optimization
## PdfOptimizationType enumeration
Specifies a type of optimization.
```csharp
public enum PdfOptimizationType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Standard | `0` | High print quality |
| MinimumSize | `1` | File size is more important than print quality |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class PdfOptimizationTypeDemo
{
public static void PdfOptimizationTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Hello World");
// Create PdfSaveOptions and set the optimization type
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;
// Save the workbook as a PDF with the specified optimization type
workbook.Save("OptimizedOutput.pdf", pdfSaveOptions);
Console.WriteLine("PDF saved with optimization type: MinimumSize");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)
