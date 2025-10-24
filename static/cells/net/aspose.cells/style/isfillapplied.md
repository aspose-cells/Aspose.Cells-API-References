##Style.IsFillApplied
Style property. Indicate whether the fill formatting should be applied
## Style.IsFillApplied property
Indicate whether the fill formatting should be applied.
```csharp
public bool IsFillApplied { get; set; }
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
public class StylePropertyIsFillAppliedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a style
Style style = workbook.CreateStyle();
// Initially, IsFillApplied should be false
Console.WriteLine("IsFillApplied (initial): " + style.IsFillApplied);
// Apply fill settings
style.ForegroundColor = Color.Yellow;
style.Pattern = BackgroundType.Solid;
// After setting fill properties, IsFillApplied should be true
Console.WriteLine("IsFillApplied (after setting fill): " + style.IsFillApplied);
// Apply the style to a cell
worksheet.Cells["A1"].SetStyle(style);
// Save the workbook
workbook.Save("IsFillAppliedDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
