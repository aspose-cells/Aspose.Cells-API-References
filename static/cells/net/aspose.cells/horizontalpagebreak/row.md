##HorizontalPageBreak.Row
HorizontalPageBreak property. Gets the zero based row index
## HorizontalPageBreak.Row property
Gets the zero based row index.
```csharp
public int Row { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HorizontalPageBreakPropertyRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add horizontal page breaks
worksheet.HorizontalPageBreaks.Add(6);
worksheet.HorizontalPageBreaks.Add(12);
// Get the horizontal page breaks collection
HorizontalPageBreakCollection breaks = worksheet.HorizontalPageBreaks;
// Display row numbers of page breaks
Console.WriteLine("Page break at row: " + breaks[0].Row);
Console.WriteLine("Page break at row: " + breaks[1].Row);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
