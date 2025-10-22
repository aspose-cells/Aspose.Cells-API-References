##HorizontalPageBreak.EndColumn
HorizontalPageBreak property. Gets the end column index of this horizontal page break
## HorizontalPageBreak.EndColumn property
Gets the end column index of this horizontal page break.
```csharp
public int EndColumn { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HorizontalPageBreakPropertyEndColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a horizontal page break at row 5, spanning from column 2 to 4
int index = worksheet.HorizontalPageBreaks.Add(5, 2, 4);
HorizontalPageBreak hPageBreak = worksheet.HorizontalPageBreaks[index];
// Display the EndColumn property
Console.WriteLine("Horizontal Page Break EndColumn: " + hPageBreak.EndColumn);
// Since EndColumn is read-only, we need to remove and re-add the page break to modify it
worksheet.HorizontalPageBreaks.RemoveAt(index);
index = worksheet.HorizontalPageBreaks.Add(5, 2, 6);
hPageBreak = worksheet.HorizontalPageBreaks[index];
Console.WriteLine("Modified Horizontal Page Break EndColumn: " + hPageBreak.EndColumn);
}
}
}
```
### See Also
* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
