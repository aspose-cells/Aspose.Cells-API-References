##Cells.GetRowHeight
Cells method. Gets rows height
## GetRowHeight(int, bool, CellsUnitType) {#getrowheight_1}
Gets row's height.
```csharp
public double GetRowHeight(int row, bool isOriginal, CellsUnitType unitType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| isOriginal | Boolean | Whether returns the original row height or 0 for hidden row. |
| unitType | CellsUnitType | Unit type of the returned height value |
### Return Value
Row's height
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodGetRowHeightWithInt32BooleanCellsUnitTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set row height for row 3 (20 pixels)
worksheet.Cells.SetRowHeightPixel(3, 20);
// Get row height in different units
double heightInPixels = worksheet.Cells.GetRowHeight(3, true, CellsUnitType.Pixel);
double heightInPoints = worksheet.Cells.GetRowHeight(3, true, CellsUnitType.Point);
// Output the results
Console.WriteLine("Row height in pixels: " + heightInPixels);
Console.WriteLine("Row height in points: " + heightInPoints);
}
}
}
```
### See Also
* enum [CellsUnitType](../../cellsunittype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetRowHeight(int) {#getrowheight}
Gets the height of a specified row, in unit of points.
```csharp
public double GetRowHeight(int row)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index |
### Return Value
Height of row
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodGetRowHeightWithInt32Demo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet ws = wb.Worksheets["Sheet1"];
Cells cells = ws.Cells;
string strText = "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.";
cells[0, 0].PutValue(strText);
Style style = cells[0, 0].GetStyle();
style.IsTextWrapped = true;
cells[0, 0].SetStyle(style);
ws.Cells.SetColumnWidth(0, 50);
ws.AutoFitRows();
double rowHeight = cells.GetRowHeight(0);
Console.WriteLine("Row height: " + rowHeight);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
