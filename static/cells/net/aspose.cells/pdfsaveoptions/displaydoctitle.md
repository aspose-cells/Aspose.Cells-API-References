##PdfSaveOptions.DisplayDocTitle
PdfSaveOptions property. Indicates whether the windows title bar should display the document title
## PdfSaveOptions.DisplayDocTitle property
Indicates whether the window's title bar should display the document title.
```csharp
public bool DisplayDocTitle { get; set; }
```
### Remarks
If false, the title bar should instead display the name of the PDF file. Default value is false.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class PdfSaveOptionsPropertyDisplayDocTitleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Aspose.Cells PDF DisplayDocTitle Example");
// Create PDF save options
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
// Set the DisplayDocTitle property to true
pdfSaveOptions.DisplayDocTitle = true;
// Save the workbook as PDF
workbook.Save("PdfDisplayDocTitleDemo.pdf", pdfSaveOptions);
}
}
}
```
### See Also
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
