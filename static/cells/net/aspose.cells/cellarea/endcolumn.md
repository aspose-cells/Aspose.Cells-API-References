##CellArea.EndColumn
CellArea field. Gets or set the end column of this area
## CellArea.EndColumn field
Gets or set the end column of this area.
```csharp
public int EndColumn;
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class CellAreaFieldEndColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create a cell area from A1 to C3
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 2;
area.EndColumn = 2;
// Process the cell area using EndColumn
ProcessCellArea(area, Color.LightBlue, sheet);
// Save the workbook
workbook.Save("CellAreaFieldEndColumnDemo_output.xlsx");
}
private static void ProcessCellArea(CellArea area, Color color, Worksheet sheet)
{
int k = 0;
for (int col = area.StartColumn; col <= area.EndColumn; col++)
{
for (int row = area.StartRow; row <= area.EndRow; row++)
{
Cell cell = sheet.Cells[row, col];
if (!color.IsEmpty)
{
Style style = cell.GetStyle();
style.ForegroundColor = color;
style.Pattern = BackgroundType.Solid;
cell.SetStyle(style);
}
cell.PutValue(row + col + k);
k++;
}
}
}
}
}
```
### See Also
* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
