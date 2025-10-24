##PptxSaveOptions.ExportViewType
PptxSaveOptions property. Gets and sets the display type when exporting to PowerPoint. The default exporting type is working as printing
## PptxSaveOptions.ExportViewType property
Gets and sets the display type when exporting to PowerPoint. The default exporting type is working as printing.
```csharp
public SlideViewType ExportViewType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;
namespace AsposeCellsExamples
{
public class PptxSaveOptionsPropertyExportViewTypeDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample Data");
// Set PPTX save options with ExportViewType
PptxSaveOptions saveOptions = new PptxSaveOptions();
saveOptions.ExportViewType = SlideViewType.View;
// Save the workbook as PPTX
workbook.Save("output.pptx", saveOptions);
Console.WriteLine("Workbook saved as PPTX with ExportViewType set to View");
}
}
}
```
### See Also
* enum [SlideViewType](../../../aspose.cells.slides/slideviewtype/)
* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
