##Cells.GetColumnWidth
Cells method. Gets the column width
## GetColumnWidth(int, bool, CellsUnitType) {#getcolumnwidth_1}
Gets the column width.
```csharp
public double GetColumnWidth(int column, bool isOriginal, CellsUnitType unitType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | The column index. |
| isOriginal | Boolean | Indicates whether getting original width. |
| unitType | CellsUnitType |  |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodGetColumnWidthWithInt32BooleanCellsUnitTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set column width for column 1 (0-based index)
cells.SetColumnWidth(0, 20);
// Get column width in different units and modes
double widthInPixels = cells.GetColumnWidth(0, true, CellsUnitType.Pixel);
double widthInPoints = cells.GetColumnWidth(0, true, CellsUnitType.Point);
double defaultWidth = cells.GetColumnWidth(0, false, CellsUnitType.Pixel);
Console.WriteLine("Column width in pixels: " + widthInPixels);
Console.WriteLine("Column width in points: " + widthInPoints);
Console.WriteLine("Default column width: " + defaultWidth);
}
}
}
```
### See Also
* enum [CellsUnitType](../../cellsunittype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetColumnWidth(int) {#getcolumnwidth}
Gets the width(in unit of characters) of the specified column in normal view
```csharp
public double GetColumnWidth(int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index |
### Return Value
Width of column. For spreadsheet, column width is measured as the number of characters of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodGetColumnWidthWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set column width for column index 255
cells.SetColumnWidth(255, 20.86);
// Get and display the column width
double columnWidth = cells.GetColumnWidth(255);
Console.WriteLine("Column width at index 255: " + columnWidth);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
