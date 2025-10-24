##Cells.GetCellStyle
Cells method. Get the style of given cell
## Cells.GetCellStyle method
Get the style of given cell.
```csharp
public Style GetCellStyle(int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | row index |
| column | Int32 | column |
### Return Value
the style of given cell.
### Remarks
The returned style is only the one set for the cell or inherited from the row/column of the cell, does not include the applied properties by other settings such as conditional formattings.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class CellsMethodGetCellStyleWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access cell B5 (row 4, column 1) and set initial style
Cell cell = worksheet.Cells["B5"];
cell.PutValue("Styled Cell");
// Create and apply initial cell style
Style initialStyle = workbook.CreateStyle();
initialStyle.Font.IsBold = true;  // Changed from Bold to IsBold
initialStyle.BackgroundColor = Color.LightYellow;
cell.SetStyle(initialStyle);
try
{
// Call GetCellStyle with Int32 parameters (row 4, column 1)
Style cellStyle = worksheet.Cells.GetCellStyle(4, 1);
// Display retrieved style properties
Console.WriteLine($"Retrieved style - Bold: {cellStyle.Font.IsBold}, Background: {cellStyle.BackgroundColor}");  // Changed from Bold to IsBold
// Modify the retrieved style
cellStyle.Font.IsItalic = true;  // Changed from Italic to IsItalic
cellStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
// Apply modified style back to the cell
cell.SetStyle(cellStyle);
Console.WriteLine("GetCellStyle executed successfully. Modified border and font style.");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetCellStyle: {ex.Message}");
}
// Save the modified workbook
workbook.Save("CellsGetCellStyleWithInt32Demo.xlsx");
}
}
}
```
### See Also
* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
