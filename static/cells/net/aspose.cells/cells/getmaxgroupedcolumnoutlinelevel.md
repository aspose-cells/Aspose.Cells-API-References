##Cells.GetMaxGroupedColumnOutlineLevel
Cells method. Gets the max grouped column outline level zerobased
## Cells.GetMaxGroupedColumnOutlineLevel method
Gets the max grouped column outline level (zero-based).
```csharp
public int GetMaxGroupedColumnOutlineLevel()
```
### Return Value
The max grouped column outline level (zero-based)
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodGetMaxGroupedColumnOutlineLevelDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Group some columns to demonstrate outline levels
cells.GroupColumns(0, 2, false);
cells.GroupColumns(3, 5, false);
// Get the maximum grouped column outline level
int maxOutlineLevel = cells.GetMaxGroupedColumnOutlineLevel();
Console.WriteLine("Maximum grouped column outline level: " + maxOutlineLevel);
// Display outline level for each column
for (int col = 0; col < 6; col++)
{
int outlineLevel = cells.GetGroupedColumnOutlineLevel(col);
Console.WriteLine($"Column {col} outline level: {outlineLevel}");
}
// Save the workbook
workbook.Save("GroupedColumnsOutlineLevel.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
