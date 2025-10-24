##HorizontalPageBreakCollection.Item
HorizontalPageBreakCollection property. Gets the HorizontalPageBreak element at the specified index
## HorizontalPageBreakCollection indexer (1 of 2)
Gets the [`HorizontalPageBreak`](../../horizontalpagebreak/) element at the specified index.
```csharp
public HorizontalPageBreak this[int index] { get; }
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
public class HorizontalPageBreakCollectionPropertyItemDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add horizontal page breaks
worksheet.HorizontalPageBreaks.Add(5);
worksheet.HorizontalPageBreaks.Add(10);
// Access page breaks using Item property
HorizontalPageBreak firstBreak = worksheet.HorizontalPageBreaks[0];
Console.WriteLine("First page break row: " + firstBreak.Row);
// Modify cells which affects page breaks
worksheet.Cells.DeleteRows(0, 2);
// Verify the page break was adjusted
Console.WriteLine("First page break after row deletion: " + worksheet.HorizontalPageBreaks[0].Row);
}
}
}
```
### See Also
* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## HorizontalPageBreakCollection indexer (2 of 2)
Gets the [`HorizontalPageBreak`](../../horizontalpagebreak/) element with the specified cell name.
```csharp
public HorizontalPageBreak this[string cellName] { get; }
```
| Parameter | Description |
| --- | --- |
| cellName | Cell name. |
### Return Value
The element with the specified cell name.
### See Also
* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
