##VerticalPageBreak.StartRow
VerticalPageBreak property. Gets the start row index of the vertical page break
## VerticalPageBreak.StartRow property
Gets the start row index of the vertical page break.
```csharp
public int StartRow { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class VerticalPageBreakPropertyStartRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add vertical page breaks with desired start row (2) initially
worksheet.VerticalPageBreaks.Add(2, 0, 10);
VerticalPageBreak vPageBreak = worksheet.VerticalPageBreaks[0];
// Display the StartRow property
Console.WriteLine("Vertical Page Break Start Row: " + vPageBreak.StartRow);
// Since StartRow is read-only, we need to remove and re-add to change it
worksheet.VerticalPageBreaks.RemoveAt(0);
worksheet.VerticalPageBreaks.Add(5, 0, 10);
vPageBreak = worksheet.VerticalPageBreaks[0];
Console.WriteLine("Modified Vertical Page Break Start Row: " + vPageBreak.StartRow);
// Save the workbook
workbook.Save("VerticalPageBreakExample.xlsx");
}
}
}
```
### See Also
* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
