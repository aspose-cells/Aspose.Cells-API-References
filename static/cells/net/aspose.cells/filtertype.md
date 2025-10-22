##Enum FilterType
Aspose.Cells.FilterType enum. The filter type
## FilterType enumeration
The filter type.
```csharp
public enum FilterType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| ColorFilter | `0` | Filter by fill color of the cell. |
| CustomFilters | `1` | Custom filter type. |
| DynamicFilter | `2` | Dynamic filter type. |
| MultipleFilters | `3` | When multiple values are chosen to filter by, or when a group of date values are chosen to filter by, this element groups those criteria together. |
| IconFilter | `4` | Filter by icon of conditional formatting. |
| Top10 | `5` | Top 10 filter. |
| None | `6` | No filter. |
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassFilterTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Color");
worksheet.Cells["A2"].PutValue("Red");
worksheet.Cells["A3"].PutValue("Green");
worksheet.Cells["A4"].PutValue("Blue");
// Create auto filter
worksheet.AutoFilter.Range = "A1:A4";
AutoFilter filter = worksheet.AutoFilter;
// Create color filter
CellsColor color = workbook.CreateCellsColor();
color.Color = Color.Red;
// Add color filter to column
filter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
filter.Refresh();
// Check filter type
FilterColumn filterColumn = filter.FilterColumns[0];
Console.WriteLine("Filter Type: " + filterColumn.FilterType);
// Verify the color filter properties
if (filterColumn.FilterType == FilterType.ColorFilter)
{
ColorFilter colorFilter = filterColumn.Filter as ColorFilter;
Console.WriteLine("Filter by fill color: " + colorFilter.FilterByFillColor);
Console.WriteLine("Filter color: " + colorFilter.GetColor(workbook.Worksheets));
}
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
