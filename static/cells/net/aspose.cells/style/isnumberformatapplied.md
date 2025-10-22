##Style.IsNumberFormatApplied
Style property. Indicate whether the number formatting should be applied
## Style.IsNumberFormatApplied property
Indicate whether the number formatting should be applied.
```csharp
public bool IsNumberFormatApplied { get; set; }
```
### Remarks
Only for named style.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyIsNumberFormatAppliedDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a style with number format
Style style = workbook.CreateStyle();
style.Number = 14; // Format as "m/d/yyyy"
style.IsNumberFormatApplied = true;
// Apply the style to a cell
Cell cell = worksheet.Cells["A1"];
cell.SetStyle(style);
// Verify the number format is applied
Console.WriteLine("IsNumberFormatApplied: " + style.IsNumberFormatApplied);
Console.WriteLine("Cell value format: " + cell.GetDisplayStyle().Number);
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
