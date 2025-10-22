##HtmlSaveOptions.SheetSet
HtmlSaveOptions property. Gets or sets the sheets to render. Default is all visible sheets in the workbook Visible
## HtmlSaveOptions.SheetSet property
Gets or sets the sheets to render. Default is all visible sheets in the workbook: [`Visible`](../../../aspose.cells.rendering/sheetset/visible/).
```csharp
public SheetSet SheetSet { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class HtmlSaveOptionsPropertySheetSetDemo
{
public static void Run()
{
// Create a new workbook with multiple worksheets
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet2");
workbook.Worksheets.Add("Sheet3");
// Make one sheet hidden for demonstration
workbook.Worksheets[1].IsVisible = false;
// Set some sample data in each sheet
for (int i = 0; i < workbook.Worksheets.Count; i++)
{
Worksheet sheet = workbook.Worksheets[i];
sheet.Cells["A1"].PutValue($"Data from {sheet.Name}");
}
// Create HtmlSaveOptions instance
HtmlSaveOptions options = new HtmlSaveOptions();
// Display current SheetSet value (default is null which means all visible sheets)
Console.WriteLine("Current SheetSet value: " + (options.SheetSet == null ? "All visible sheets" : "Custom set"));
// Set SheetSet to only include specific sheets (by index)
options.SheetSet = new SheetSet(new int[] { 0, 2 });
// Save to HTML - only the specified sheets will be included
workbook.Save("HtmlWithCustomSheetSet.html", options);
// Change SheetSet to only visible sheets
options.SheetSet = SheetSet.Visible;
workbook.Save("HtmlWithVisibleSheets.html", options);
// Change SheetSet to active sheet only
workbook.Worksheets[2].IsSelected = true; // Activate the sheet by selecting it
options.SheetSet = SheetSet.Active;
workbook.Save("HtmlWithActiveSheet.html", options);
}
}
}
```
### See Also
* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
