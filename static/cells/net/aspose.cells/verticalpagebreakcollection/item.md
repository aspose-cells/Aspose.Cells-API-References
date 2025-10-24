##VerticalPageBreakCollection.Item
VerticalPageBreakCollection property. Gets the VerticalPageBreak element at the specified index
## VerticalPageBreakCollection indexer (1 of 2)
Gets the [`VerticalPageBreak`](../../verticalpagebreak/) element at the specified index.
```csharp
public VerticalPageBreak this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |
### Return Value
The element at the specified index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class VerticalPageBreakCollectionPropertyItemDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add vertical page breaks
worksheet.VerticalPageBreaks.Add(5);
worksheet.VerticalPageBreaks.Add(10);
worksheet.VerticalPageBreaks.Add(15);
// Access and display page breaks using Item property
VerticalPageBreakCollection vpagebreaks = worksheet.VerticalPageBreaks;
Console.WriteLine("Vertical Page Breaks:");
for (int i = 0; i < vpagebreaks.Count; i++)
{
Console.WriteLine($"Break {i + 1}: Column = {vpagebreaks[i].Column}");
}
// Remove and re-add to modify a page break since Column is read-only
int column = vpagebreaks[1].Column;
vpagebreaks.RemoveAt(1);
vpagebreaks.Add(12);
Console.WriteLine("\nAfter modification:");
Console.WriteLine($"Break 2: Column = {vpagebreaks[1].Column}");
}
}
}
```
### See Also
* class [VerticalPageBreak](../../verticalpagebreak/)
* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## VerticalPageBreakCollection indexer (2 of 2)
Gets the [`VerticalPageBreak`](../../verticalpagebreak/) element with the specified cell name.
```csharp
public VerticalPageBreak this[string cellName] { get; }
```
| Parameter | Description |
| --- | --- |
| cellName | Cell name. |
### Return Value
The element with the specified cell name.
### See Also
* class [VerticalPageBreak](../../verticalpagebreak/)
* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
