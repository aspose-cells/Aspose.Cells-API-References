##Style.IsTextWrapped
Style property. Gets or sets a value indicating whether the text within a cell is wrapped
## Style.IsTextWrapped property
Gets or sets a value indicating whether the text within a cell is wrapped.
```csharp
public bool IsTextWrapped { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyIsTextWrappedDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet ws = wb.Worksheets[0];
Cells cells = ws.Cells;
// Set long text in cell
Cell cell = cells["A1"];
cell.PutValue("This is a long text that should be wrapped in the cell");
// Enable text wrapping
Style style = cell.GetStyle();
style.IsTextWrapped = true;
cell.SetStyle(style);
// Adjust row height to show wrapped text
ws.AutoFitRow(0);
// Save the workbook
wb.Save("output.xlsx");
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
