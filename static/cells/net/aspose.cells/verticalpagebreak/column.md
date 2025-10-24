##VerticalPageBreak.Column
VerticalPageBreak property. Gets the column index of the vertical page break
## VerticalPageBreak.Column property
Gets the column index of the vertical page break.
```csharp
public int Column { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class VerticalPageBreakPropertyColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add vertical page breaks at columns 4 and 8
worksheet.VerticalPageBreaks.Add(4);
worksheet.VerticalPageBreaks.Add(8);
// Get the vertical page breaks collection
VerticalPageBreakCollection vpagebreaks = worksheet.VerticalPageBreaks;
// Display information about each vertical page break
Console.WriteLine("Vertical Page Breaks Count: " + vpagebreaks.Count);
foreach (VerticalPageBreak vpagebreak in vpagebreaks)
{
Console.WriteLine("\nPage Break at Column: " + vpagebreak.Column);
Console.WriteLine("Start Row: " + vpagebreak.StartRow);
Console.WriteLine("End Row: " + vpagebreak.EndRow);
}
// Save the workbook
workbook.Save("VerticalPageBreakDemo.xlsx");
}
}
}
```
### See Also
* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
