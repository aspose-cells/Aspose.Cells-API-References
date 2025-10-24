##PaginatedSaveOptions.SheetSet
PaginatedSaveOptions property. Gets or sets the sheets to render. Default is all visible sheets in the workbook Visible
## PaginatedSaveOptions.SheetSet property
Gets or sets the sheets to render. Default is all visible sheets in the workbook: [`Visible`](../../../aspose.cells.rendering/sheetset/visible/).
```csharp
public SheetSet SheetSet { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class PaginatedSaveOptionsPropertySheetSetDemo
{
public static void Run()
{
// Create a new workbook with two worksheets
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet2");
// Set some sample data in both sheets
workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");
// Create PDF save options
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
// Save only the second sheet using SheetSet
pdfSaveOptions.SheetSet = new SheetSet(new int[] { 1 }); // 0-based index
// Save the workbook with the specified sheets
workbook.Save("output.pdf", pdfSaveOptions);
}
}
}
```
### See Also
* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
