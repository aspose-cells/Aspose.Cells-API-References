##Cell.GetDisplayStyle
Cell method. Gets the display style of this cell
## GetDisplayStyle() {#getdisplaystyle}
Gets the display style of this cell.
```csharp
public Style GetDisplayStyle()
```
### Return Value
display style of this cell
### Remarks
Same with using SideBorders for `GetDisplayStyle`. That is, this method will check and adjust top/bottom/left/right borders of this cell according to the style([`GetStyle`](../getstyle/)) of its adjacent cells, but do not check the merged cells, and do not check the display style of adjacent cells.
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class CellMethodGetDisplayStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set style for cell A1
Style style1 = workbook.CreateStyle();
style1.ForegroundColor = Color.FromArgb(157, 195, 230);
worksheet.Cells["A1"].SetStyle(style1);
// Set style for cell A23
Style style2 = workbook.CreateStyle();
style2.ForegroundColor = Color.Red;
worksheet.Cells["A23"].SetStyle(style2);
// Get and display styles
Style displayStyle1 = worksheet.Cells["A1"].GetDisplayStyle();
Console.WriteLine("A1 Foreground Color: " + displayStyle1.ForegroundColor);
Style displayStyle2 = worksheet.Cells["A23"].GetDisplayStyle();
Console.WriteLine("A23 Foreground Color: " + displayStyle2.ForegroundColor);
}
}
}
```
### See Also
* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetDisplayStyle(bool) {#getdisplaystyle_2}
Gets the display style of this cell.
```csharp
public Style GetDisplayStyle(bool includeMergedBorders)
```
| Parameter | Type | Description |
| --- | --- | --- |
| includeMergedBorders | Boolean | Indicates whether checking borders of merged cells. |
### Return Value
display style of this cell
### Remarks
If the specified flag is false, then it is same with `GetDisplayStyle`. Otherwise it is same with using SideBorders&#x7C;DynamicStyleBorders for `GetDisplayStyle`.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodGetDisplayStyleWithBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access cell B2 and set some style properties
Cell cell = worksheet.Cells["B2"];
Style cellStyle = cell.GetStyle();
cellStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
cell.SetStyle(cellStyle);
// Get display style with formatting (true parameter)
Style displayStyle = cell.GetDisplayStyle(true);
// Output the right border line style
Console.WriteLine("Right Border Line Style: " + displayStyle.Borders[BorderType.RightBorder].LineStyle);
}
}
}
```
### See Also
* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetDisplayStyle(BorderType) {#getdisplaystyle_1}
Gets the display style of this cell.
```csharp
public Style GetDisplayStyle(BorderType adjacentBorders)
```
| Parameter | Type | Description |
| --- | --- | --- |
| adjacentBorders | BorderType | Indicates which borders need to be checked and adjusted according to the borders of adjacent cells. |
### Return Value
display style of this cell
### Remarks
If this cell is also affected by other settings such as conditional formatting, list objects, etc., then the display style may be different from [`GetStyle`](../getstyle/). For flags of adjusting borders according to adjacent cells, TopBorder/BottomBorder /LeftBorder/RightBorder denote whether check and combine the bottom/top/right/left borders of the left/right/top/bottom cells adjacent to this one. For performance and compatibility consideration, some enums are used to denote some special operations: Horizontal/Vertical denote whether check and combine the bottom/right border of merged cells to this one. Diagonal(that is, both DiagonalUpBorder and DiagonalDownBorder have been set) denotes check and combine borders from the display style of adjacent cells. Please note, checking borders/styles of adjacent cells, especially the display styles, is time-consumed process. If there is no need to get the borders for the returned style, using None to disable the process of adjacent cells will give better performance. When getting borders of adjacent cells from styles defined on those cells only(without setting Diagonal), the performance also may be better because checking the display style of one cell is time-consumed too.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodGetDisplayStyleWithBorderTypeDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
Cells cells = sheet.Cells;
// Set sample data
for (int i = 0; i < 10; i++)
{
cells[i, 0].PutValue(i);
}
// Create conditional formatting
FormatConditionCollection fcs = sheet.ConditionalFormattings[sheet.ConditionalFormattings.Add()];
fcs.AddArea(CellArea.CreateCellArea(0, 0, 9, 0));
fcs.AddCondition(FormatConditionType.ColorScale);
// Get display style with different border types
for (int i = 0; i < 10; i++)
{
Style styleWithBorder = cells[i, 0].GetDisplayStyle(BorderType.TopBorder);
Style styleWithoutBorder = cells[i, 0].GetDisplayStyle(BorderType.None);
Console.WriteLine($"Cell {i + 1}:");
Console.WriteLine($"  Style with border - Foreground: {styleWithBorder.ForegroundArgbColor:X}");
Console.WriteLine($"  Style without border - Foreground: {styleWithoutBorder.ForegroundArgbColor:X}");
}
}
}
}
```
### See Also
* class [Style](../../style/)
* enum [BorderType](../../bordertype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
