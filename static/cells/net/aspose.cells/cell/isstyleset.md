##Cell.IsStyleSet
Cell property. Indicates if the cells style is set. If return false it means this cell has a default cell format
## Cell.IsStyleSet property
Indicates if the cell's style is set. If return false, it means this cell has a default cell format.
```csharp
public bool IsStyleSet { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyIsStyleSetDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Access a cell that hasn't been styled yet
Cell unsetStyleCell = cells["A1"];
Console.WriteLine($"Cell A1 IsStyleSet before styling: {unsetStyleCell.IsStyleSet}");
// Style a different cell
Cell styledCell = cells["B2"];
Style style = workbook.CreateStyle();
style.Font.Name = "Arial";
style.Font.Size = 12;
styledCell.SetStyle(style);
Console.WriteLine($"Cell B2 IsStyleSet after styling: {styledCell.IsStyleSet}");
// Check if style is inherited from row
Row row = cells.Rows[4];
row.SetStyle(style);
Cell rowInheritedCell = cells["E4"];
Console.WriteLine($"Cell E4 IsStyleSet (inherited from row): {rowInheritedCell.IsStyleSet}");
// Explicitly set style to null for a cell
Cell nullStyleCell = cells["C3"];
nullStyleCell.SetStyle(null);
Console.WriteLine($"Cell C3 IsStyleSet after setting null: {nullStyleCell.IsStyleSet}");
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
