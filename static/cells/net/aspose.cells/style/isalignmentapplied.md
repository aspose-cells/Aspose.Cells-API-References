##Style.IsAlignmentApplied
Style property. Indicate whether the alignment formatting should be applied
## Style.IsAlignmentApplied property
Indicate whether the alignment formatting should be applied.
```csharp
public bool IsAlignmentApplied { get; set; }
```
### Remarks
Only for named style.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyIsAlignmentAppliedDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cell cell = worksheet.Cells["A1"];
Style style = cell.GetStyle();
// Set alignment properties
style.HorizontalAlignment = TextAlignmentType.Center;
style.VerticalAlignment = TextAlignmentType.Center;
// Enable alignment application
style.IsAlignmentApplied = true;
cell.SetStyle(style);
// Verify alignment is applied
Console.WriteLine("Alignment applied: " + style.IsAlignmentApplied);
Console.WriteLine("Horizontal Alignment: " + style.HorizontalAlignment);
Console.WriteLine("Vertical Alignment: " + style.VerticalAlignment);
workbook.Save("AlignmentExample.xlsx");
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
