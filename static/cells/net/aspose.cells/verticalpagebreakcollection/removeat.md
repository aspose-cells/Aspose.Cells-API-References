##VerticalPageBreakCollection.RemoveAt
VerticalPageBreakCollection method. Removes the VPageBreak element at a specified name
## VerticalPageBreakCollection.RemoveAt method
Removes the VPageBreak element at a specified name.
```csharp
public void RemoveAt(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | Element index, zero based. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class VerticalPageBreakCollectionMethodRemoveAtWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;
verticalPageBreaks.Add(0, 10, 2);
verticalPageBreaks.Add(4);
verticalPageBreaks.Add(5, 3);
verticalPageBreaks.Add("G5");
verticalPageBreaks.RemoveAt(1);
for (int i = 0; i < verticalPageBreaks.Count; i++)
{
VerticalPageBreak vpb = verticalPageBreaks[i];
Console.WriteLine($"Vertical Page Break {i}: Column = {vpb.Column}, StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}");
}
workbook.Save("VerticalPageBreakCollectionExample.xlsx");
}
}
}
```
### See Also
* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
