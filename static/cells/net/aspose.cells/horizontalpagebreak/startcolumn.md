##HorizontalPageBreak.StartColumn
HorizontalPageBreak property. Gets the start column index of this horizontal page break
## HorizontalPageBreak.StartColumn property
Gets the start column index of this horizontal page break.
```csharp
public int StartColumn { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HorizontalPageBreakPropertyStartColumnDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add page breaks at different columns to demonstrate StartColumn
int index1 = worksheet.HorizontalPageBreaks.Add("Y30");
int index2 = worksheet.HorizontalPageBreaks.Add("B30");
HorizontalPageBreak hPageBreak1 = worksheet.HorizontalPageBreaks[index1];
HorizontalPageBreak hPageBreak2 = worksheet.HorizontalPageBreaks[index2];
Console.WriteLine($"First Break Start Column: {hPageBreak1.StartColumn}");
Console.WriteLine($"Second Break Start Column: {hPageBreak2.StartColumn}");
workbook.Save("HorizontalPageBreakExample.xlsx");
}
}
}
```
### See Also
* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
