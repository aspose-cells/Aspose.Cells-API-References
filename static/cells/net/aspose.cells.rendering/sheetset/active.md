##SheetSet.Active
SheetSet property. Gets a set with active sheet of the workbook
## SheetSet.Active property
Gets a set with active sheet of the workbook.
```csharp
public static SheetSet Active { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class SheetSetPropertyActiveDemo
{
public static void Run()
{
// Create a new workbook with two worksheets
Workbook workbook = new Workbook();
workbook.Worksheets.Add();
// Set the second worksheet as active
workbook.Worksheets.ActiveSheetIndex = 1;
// Add data to both worksheets
workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
workbook.Worksheets[1].Cells["A1"].PutValue("Active Sheet Data");
// Create PDF save options
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
// Save only the active sheet
pdfSaveOptions.SheetSet = SheetSet.Active;
workbook.Save("ActiveSheetOnly.pdf", pdfSaveOptions);
// Save all sheets for comparison
pdfSaveOptions.SheetSet = SheetSet.All;
workbook.Save("AllSheets.pdf", pdfSaveOptions);
}
}
}
```
### See Also
* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
