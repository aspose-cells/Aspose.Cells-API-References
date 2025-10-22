##Style.IsBorderApplied
Style property. Indicate whether the border formatting should be applied
## Style.IsBorderApplied property
Indicate whether the border formatting should be applied.
```csharp
public bool IsBorderApplied { get; set; }
```
### Remarks
Only for named style.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyIsBorderAppliedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a custom style
Style style = workbook.CreateStyle();
// Apply border settings to the style
style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Black;
// Check if border is applied
Console.WriteLine("IsBorderApplied before setting: " + style.IsBorderApplied);
// Explicitly set IsBorderApplied to true
style.IsBorderApplied = true;
// Apply the style to a cell
worksheet.Cells["A1"].SetStyle(style);
// Verify border application
Console.WriteLine("IsBorderApplied after setting: " + style.IsBorderApplied);
// Save the workbook
workbook.Save("IsBorderAppliedDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
