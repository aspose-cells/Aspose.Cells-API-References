##PdfSaveOptions.CreatedTime
PdfSaveOptions property. Gets and sets the time of generating the pdf document
## PdfSaveOptions.CreatedTime property
Gets and sets the time of generating the pdf document.
```csharp
public DateTime CreatedTime { get; set; }
```
### Remarks
if it is not be set, it will be the time of generating the pdf.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class PdfSaveOptionsPropertyCreatedTimeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Worksheets[0].Cells["A1"].PutValue("PDF with CreatedTime demonstration");
PdfSaveOptions saveOptions = new PdfSaveOptions
{
CreatedTime = DateTime.Now,
Compliance = PdfCompliance.PdfA1b
};
string outputPath = "OutputWithCreatedTime.pdf";
workbook.Save(outputPath, saveOptions);
Console.WriteLine($"PDF saved with CreatedTime: {saveOptions.CreatedTime}");
}
}
}
```
### See Also
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
