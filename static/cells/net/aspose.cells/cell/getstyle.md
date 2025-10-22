##Cell.GetStyle
Cell method. Gets the cell style
## GetStyle() {#getstyle}
Gets the cell style.
```csharp
public Style GetStyle()
```
### Return Value
Style object.
### Remarks
To change the style of the cell, please call Cell.SetStyle() method after modifying the returned style object. This method is same with `GetStyle` with true value for the parameter.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodGetStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set different vertical alignments for cells
cells["A1"].PutValue("Bottom Alignment");
cells["A1"].GetStyle().VerticalAlignment = TextAlignmentType.Bottom;
cells["A2"].PutValue("Center Alignment");
cells["A2"].GetStyle().VerticalAlignment = TextAlignmentType.Center;
cells["A3"].PutValue("Distributed Alignment");
cells["A3"].GetStyle().VerticalAlignment = TextAlignmentType.Distributed;
cells["A4"].PutValue("Justify Alignment");
cells["A4"].GetStyle().VerticalAlignment = TextAlignmentType.Justify;
cells["A5"].PutValue("Top Alignment");
cells["A5"].GetStyle().VerticalAlignment = TextAlignmentType.Top;
// Demonstrate GetStyle() method
Console.WriteLine("A1 Vertical Alignment: " + cells["A1"].GetStyle().VerticalAlignment);
Console.WriteLine("A2 Vertical Alignment: " + cells["A2"].GetStyle().VerticalAlignment);
Console.WriteLine("A3 Vertical Alignment: " + cells["A3"].GetStyle().VerticalAlignment);
Console.WriteLine("A4 Vertical Alignment: " + cells["A4"].GetStyle().VerticalAlignment);
Console.WriteLine("A5 Vertical Alignment: " + cells["A5"].GetStyle().VerticalAlignment);
}
}
}
```
### See Also
* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetStyle(bool) {#getstyle_1}
If checkBorders is true, check whether other cells' borders will effect the style of this cell.
```csharp
public Style GetStyle(bool checkBorders)
```
| Parameter | Type | Description |
| --- | --- | --- |
| checkBorders | Boolean | Check other cells' borders |
### Return Value
Style object.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodGetStyleWithBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access a cell and set some sample data
Cell cell = worksheet.Cells["A1"];
cell.PutValue(123.456);
// Get the cell's style without inheriting from row/column (false parameter)
Style style = cell.GetStyle(false);
// Modify the style
style.Custom = "0.000";
style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.None;
// Apply the modified style to the cell
cell.SetStyle(style);
// Verify the style changes
Console.WriteLine("Number Format: " + cell.GetStyle(false).Custom);
Console.WriteLine("Top Border Style: " + cell.GetStyle(false).Borders[BorderType.TopBorder].LineStyle);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
