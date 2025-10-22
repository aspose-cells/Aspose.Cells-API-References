##Worksheet.CellWatches
Worksheet property. Gets collection of cells on this worksheet being watched in the watch window
## Worksheet.CellWatches property
Gets collection of cells on this worksheet being watched in the 'watch window'.
```csharp
public CellWatchCollection CellWatches { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyCellWatchesDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data to cell B2
sheet.Cells["B2"].PutValue("Sample Data");
// Add Cell Watch for B2
int watchIndex = sheet.CellWatches.Add("B2");
CellWatch cellWatch = sheet.CellWatches[watchIndex];
// Display watch information
Console.WriteLine($"Cell Watch Added - Index: {watchIndex}");
Console.WriteLine($"Cell Name: {cellWatch.CellName}");
Console.WriteLine($"Row: {cellWatch.Row}, Column: {cellWatch.Column}");
// Save the workbook
workbook.Save("CellWatchDemo.xlsx");
}
}
}
```
### See Also
* class [CellWatchCollection](../../cellwatchcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
