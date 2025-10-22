##Cells.GetMaxGroupedRowOutlineLevel
Cells method. Gets the max grouped row outline level zerobased
## Cells.GetMaxGroupedRowOutlineLevel method
Gets the max grouped row outline level (zero-based).
```csharp
public int GetMaxGroupedRowOutlineLevel()
```
### Return Value
The max grouped row outline level (zero-based)
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodGetMaxGroupedRowOutlineLevelDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Group some rows to demonstrate outline levels
cells.GroupRows(0, 2, false);
cells.GroupRows(4, 6, false);
// Add nested grouping
cells.GroupRows(4, 5, true);
// Get the maximum grouped row outline level
int maxOutlineLevel = cells.GetMaxGroupedRowOutlineLevel();
// Display the result
Console.WriteLine("Maximum grouped row outline level: " + maxOutlineLevel);
// Display outline level for each row
for (int row = 0; row <= 6; row++)
{
Console.WriteLine($"Row {row} outline level: {cells.GetGroupedRowOutlineLevel(row)}");
}
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
