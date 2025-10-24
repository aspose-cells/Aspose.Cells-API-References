##CellWatchCollection.Item
CellWatchCollection property. Gets and sets CellWatch by index
## CellWatchCollection indexer (1 of 2)
Gets and sets [`CellWatch`](../../cellwatch/) by index.
```csharp
public CellWatch this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellWatchCollectionPropertyItemDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
int watchIndex = sheet.CellWatches.Add("B2");
CellWatchCollection cellWatches = sheet.CellWatches;
// Demonstrate Item property usage
CellWatch cellWatch = cellWatches[watchIndex];
Console.WriteLine("Cell Watch Details:");
Console.WriteLine($"Row: {cellWatch.Row}");
Console.WriteLine($"Column: {cellWatch.Column}");
Console.WriteLine($"Cell Name: {cellWatch.CellName}");
cellWatch.Row = 1;
cellWatch.Column = 1;
cellWatch.CellName = "A1";
Console.WriteLine("\nModified Cell Watch Details:");
Console.WriteLine($"Row: {cellWatch.Row}");
Console.WriteLine($"Column: {cellWatch.Column}");
Console.WriteLine($"Cell Name: {cellWatch.CellName}");
workbook.Save("CellWatchCollectionExample.xlsx");
}
}
}
```
### See Also
* class [CellWatch](../../cellwatch/)
* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## CellWatchCollection indexer (2 of 2)
Gets and sets [`CellWatch`](../../cellwatch/) by the name of the cell.
```csharp
public CellWatch this[string cellName] { get; }
```
| Parameter | Description |
| --- | --- |
| cellName | The name of the cell. |
### See Also
* class [CellWatch](../../cellwatch/)
* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
