##Style.IsFontApplied
Style property. Indicate whether the font formatting should be applied
## Style.IsFontApplied property
Indicate whether the font formatting should be applied.
```csharp
public bool IsFontApplied { get; set; }
```
### Remarks
Only for named style.
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class StylePropertyIsFontAppliedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access a cell from the worksheet
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Sample Text");
// Get the style of the cell
Style style = cell.GetStyle();
// Apply font settings
style.Font.Name = "Times New Roman";
style.Font.Size = 14;
style.Font.Color = Color.Blue;
// Enable font application
style.IsFontApplied = true;
// Set the modified style back to the cell
cell.SetStyle(style);
// Save the workbook
workbook.Save("FontAppliedDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
