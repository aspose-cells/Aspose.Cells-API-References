##ColorFilter.GetColor
ColorFilter method. Gets the color of this filter
## ColorFilter.GetColor method
Gets the color of this filter.
```csharp
public Color GetColor(WorksheetCollection sheets)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheets | WorksheetCollection |  |
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class ColorFilterMethodGetColorWithWorksheetCollectionDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Header");
worksheet.Cells["A2"].PutValue("Item 1");
worksheet.Cells["A3"].PutValue("Item 2");
worksheet.Cells["A4"].PutValue("Item 3");
// Create auto filter
worksheet.AutoFilter.Range = "A1:A4";
// Create color filter
CellsColor color = workbook.CreateCellsColor();
color.Color = Color.Red;
worksheet.AutoFilter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
worksheet.AutoFilter.Refresh();
// Get the color filter and verify its color
FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
ColorFilter colorFilter = filterColumn.Filter as ColorFilter;
if (colorFilter != null)
{
Color retrievedColor = colorFilter.GetColor(workbook.Worksheets);
Console.WriteLine("Filter color: " + retrievedColor.ToString());
}
}
}
}
```
### See Also
* class [WorksheetCollection](../../worksheetcollection/)
* class [ColorFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
