##ColorFilter.FilterByFillColor
ColorFilter property. Whether filter by the cells fill color
## ColorFilter.FilterByFillColor property
Whether filter by the cell's fill color.
```csharp
public bool FilterByFillColor { get; set; }
```
### Remarks
True: cell's fill color; False: cell's font color.
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class ColorFilterPropertyFilterByFillColorDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add sample data with different fill colors
cells["A1"].PutValue("Header");
cells["A2"].PutValue("Data1");
cells["A3"].PutValue("Data2");
cells["A4"].PutValue("Data3");
// Set fill colors
Style style1 = cells["A2"].GetStyle();
style1.ForegroundColor = Color.Red;
style1.Pattern = BackgroundType.Solid;
cells["A2"].SetStyle(style1);
Style style2 = cells["A3"].GetStyle();
style2.ForegroundColor = Color.Blue;
style2.Pattern = BackgroundType.Solid;
cells["A3"].SetStyle(style2);
Style style3 = cells["A4"].GetStyle();
style3.ForegroundColor = Color.Green;
style3.Pattern = BackgroundType.Solid;
cells["A4"].SetStyle(style3);
// Apply auto filter
worksheet.AutoFilter.Range = "A1:A4";
AutoFilter filter = worksheet.AutoFilter;
// Create color filter for fill color
CellsColor color = workbook.CreateCellsColor();
color.Color = Color.Red;
filter.AddFillColorFilter(0, BackgroundType.Solid, color, null);
filter.Refresh();
// Verify filter settings
FilterColumn filterColumn = filter.FilterColumns[0];
ColorFilter colorFilter = filterColumn.Filter as ColorFilter;
// Demonstrate FilterByFillColor property
Console.WriteLine("FilterByFillColor: " + colorFilter.FilterByFillColor); // Should be True
Console.WriteLine("Filtered rows:");
for (int row = 1; row <= 3; row++)
{
Console.WriteLine($"Row {row} hidden: {cells.IsRowHidden(row)}");
}
}
}
}
```
### See Also
* class [ColorFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
