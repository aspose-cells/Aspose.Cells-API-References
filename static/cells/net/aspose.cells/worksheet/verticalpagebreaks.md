##Worksheet.VerticalPageBreaks
Worksheet property. Gets the VerticalPageBreakCollection collection
## Worksheet.VerticalPageBreaks property
Gets the [`VerticalPageBreakCollection`](../../verticalpagebreakcollection/) collection.
```csharp
public VerticalPageBreakCollection VerticalPageBreaks { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyVerticalPageBreaksDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;
// Add different types of vertical page breaks
verticalPageBreaks.Add(0, 10, 2);
verticalPageBreaks.Add(4);
verticalPageBreaks.Add(5, 3);
verticalPageBreaks.Add("G5");
// Remove one break
verticalPageBreaks.RemoveAt(1);
// Print break information
for (int i = 0; i < verticalPageBreaks.Count; i++)
{
VerticalPageBreak vpb = verticalPageBreaks[i];
Console.WriteLine($"Break {i}: StartRow={vpb.StartRow}, EndRow={vpb.EndRow}, Column={vpb.Column}");
}
workbook.Save("VerticalPageBreaksDemo.xlsx");
}
}
}
```
### See Also
* class [VerticalPageBreakCollection](../../verticalpagebreakcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
