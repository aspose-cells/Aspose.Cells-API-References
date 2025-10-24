##PaginatedSaveOptions.GridlineType
PaginatedSaveOptions property. Gets or sets gridline type
## PaginatedSaveOptions.GridlineType property
Gets or sets gridline type.
```csharp
public GridlineType GridlineType { get; set; }
```
### Remarks
Default is Dotted type.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class PaginatedSaveOptionsPropertyGridlineTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and enable gridlines
worksheet.Cells["A1"].PutValue("GridlineType Demo");
worksheet.Cells["B2"].PutValue(1);
worksheet.Cells["C3"].PutValue(2);
worksheet.Cells["D4"].PutValue(3);
worksheet.IsGridlinesVisible = true;
// Create PDF save options
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
// Demonstrate GridlineType property
pdfSaveOptions.GridlineType = GridlineType.Dotted;
// Save the workbook with gridlines
workbook.Save("GridlineTypeDemo.pdf", pdfSaveOptions);
}
}
}
```
### See Also
* enum [GridlineType](../../gridlinetype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
