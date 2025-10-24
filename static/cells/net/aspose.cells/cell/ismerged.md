##Cell.IsMerged
Cell property. Checks if a cell is part of a merged range or not
## Cell.IsMerged property
Checks if a cell is part of a merged range or not.
```csharp
public bool IsMerged { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyIsMergedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Merge cells A1 to B2
worksheet.Cells.Merge(0, 0, 2, 2);
// Check if cell A1 is merged
bool isMerged = worksheet.Cells["A1"].IsMerged;
Console.WriteLine("Is cell A1 merged? " + isMerged);
// Check if cell C1 is merged (should be false)
isMerged = worksheet.Cells["C1"].IsMerged;
Console.WriteLine("Is cell C1 merged? " + isMerged);
// Save the workbook
workbook.Save("MergedCellsDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
