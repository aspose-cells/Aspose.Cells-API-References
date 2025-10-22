##Cells.GetCellDisplayStyle
Cells method. Get the display style of given cell
## GetCellDisplayStyle(int, int) {#getcelldisplaystyle}
Get the display style of given cell.
```csharp
public Style GetCellDisplayStyle(int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | row index of given cell |
| column | Int32 | column of given cell |
### Return Value
the display style of given cell.
### Remarks
Same with [`GetDisplayStyle`](../../cell/getdisplaystyle/), and same with using SideBorders for `GetCellDisplayStyle`.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodGetCellDisplayStyleWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Prepare cell style for demonstration
Cell cell = cells[0, 0];
cell.PutValue("Style Demo");
// Create custom style
Style style = workbook.CreateStyle();
style.Font.IsBold = true;
style.ForegroundColor = System.Drawing.Color.Yellow;
style.Pattern = BackgroundType.Solid;
// Apply style to cell
cell.SetStyle(style);
try
{
// Call GetCellDisplayStyle with row 0 and column 0
Style displayStyle = cells.GetCellDisplayStyle(0, 0);
// Display style properties
Console.WriteLine($"Bold: {displayStyle.Font.IsBold}");
Console.WriteLine($"Background Color: {displayStyle.ForegroundColor}");
// Apply the display style to another cell for visual verification
cells[2, 2].SetStyle(displayStyle);
cells[2, 2].PutValue("Style Copied");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetCellDisplayStyle method: {ex.Message}");
}
// Save the workbook
workbook.Save("CellsMethodGetCellDisplayStyleWithInt32Int32Demo.xlsx");
}
}
}
```
### See Also
* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetCellDisplayStyle(int, int, BorderType) {#getcelldisplaystyle_1}
Get the display style of given cell.
```csharp
public Style GetCellDisplayStyle(int row, int column, BorderType adjacentBorders)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | row index of given cell |
| column | Int32 | column of given cell |
| adjacentBorders | BorderType | Indicates which borders need to be checked and adjusted according to the borders of adjacent cells. Please see the description for the same parameter of [`GetDisplayStyle`](../../cell/getdisplaystyle/). |
### Return Value
the display style of given cell.
### Remarks
If the cell is also affected by other settings such as conditional formatting, list objects, etc., then the display style may be different from [`GetCellStyle`](../getcellstyle/). And because those settings also may be applied to empty(non-existing) cells, using this method can avoid the instantiation of those empty cells so the performance will be better than getting the Cell instance from Cells and then calling [`GetDisplayStyle`](../../cell/getdisplaystyle/).
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodGetCellDisplayStyleWithInt32Int32BorderTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access cell A1 and set a border style
Cell cell = worksheet.Cells["A1"];
Style style = cell.GetStyle();
style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
cell.SetStyle(style);
try
{
// Call GetCellDisplayStyle with specific parameters (0,0 for A1, TopBorder type)
Style displayStyle = worksheet.Cells.GetCellDisplayStyle(0, 0, BorderType.TopBorder);
// Check if the retrieved style matches our border color
if (displayStyle.Borders[BorderType.TopBorder].Color == System.Drawing.Color.Red)
{
Console.WriteLine("Top border display style retrieved successfully - Color: Red");
}
// Demonstrate style application by modifying another cell
Cell targetCell = worksheet.Cells["B1"];
targetCell.SetStyle(displayStyle);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetCellDisplayStyle method: {ex.Message}");
}
// Save the result
workbook.Save("GetCellDisplayStyleWithBorderTypeDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../../style/)
* enum [BorderType](../../bordertype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
