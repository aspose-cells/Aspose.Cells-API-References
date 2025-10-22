##MarkdownSaveOptions.SheetSet
MarkdownSaveOptions property. Gets or sets the sheets to render. Default is all visible sheets in the workbook Active
## MarkdownSaveOptions.SheetSet property
Gets or sets the sheets to render. Default is all visible sheets in the workbook: [`Active`](../../../aspose.cells.rendering/sheetset/active/).
```csharp
public SheetSet SheetSet { get; set; }
```
### Remarks
The set is ignored when it is used in [`SheetRender`](../../../aspose.cells.rendering/sheetrender/)
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markdown;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class MarkdownSaveOptionsPropertySheetSetDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet sheet1 = workbook.Worksheets[0];
sheet1.Cells["A1"].PutValue("Sheet1 Data");
// Add a second worksheet
Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
sheet2.Cells["A1"].PutValue("Sheet2 Data");
// Create Markdown save options
MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;
// Save all sheets to markdown
saveOptions.SheetSet = SheetSet.All;
workbook.Save("output_all_sheets.md", saveOptions);
// Save only the first sheet
saveOptions.SheetSet = new SheetSet(new int[] { 0 });
workbook.Save("output_first_sheet.md", saveOptions);
}
}
}
```
### See Also
* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
