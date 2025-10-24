##Cells.IsDefaultRowHeightMatched
Cells property. Indicates that row height and default font height matches
## Cells.IsDefaultRowHeightMatched property
Indicates that row height and default font height matches
```csharp
public bool IsDefaultRowHeightMatched { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyIsDefaultRowHeightMatchedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Set and demonstrate IsDefaultRowHeightMatched property
cells.IsDefaultRowHeightMatched = true;
Console.WriteLine("IsDefaultRowHeightMatched: " + cells.IsDefaultRowHeightMatched);
// Save the workbook
workbook.Save("output.xlsx");
// Load the saved workbook to verify the property
Workbook loadedWorkbook = new Workbook("output.xlsx");
Cells loadedCells = loadedWorkbook.Worksheets[0].Cells;
Console.WriteLine("Loaded IsDefaultRowHeightMatched: " + loadedCells.IsDefaultRowHeightMatched);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
