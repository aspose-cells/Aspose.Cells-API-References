##AutoFilter.AddFillColorFilter
AutoFilter method. Adds a fill color filter
## AutoFilter.AddFillColorFilter method
Adds a fill color filter.
```csharp
public void AddFillColorFilter(int fieldIndex, BackgroundType pattern, CellsColor foregroundColor,
CellsColor backgroundColor)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| pattern | BackgroundType | The background pattern type. |
| foregroundColor | CellsColor | The foreground color. |
| backgroundColor | CellsColor | The background color. |
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class AutoFilterMethodAddFillColorFilterWithInt32BackgroundTypeCellsColorCDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data with different fill colors
Cells cells = worksheet.Cells;
cells["A1"].PutValue("Header");
cells["A2"].PutValue("Data1");
cells["A3"].PutValue("Data2");
cells["A4"].PutValue("Data3");
// Apply different fill colors
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
// Create auto filter
worksheet.AutoFilter.Range = "A1:A4";
AutoFilter filter = worksheet.AutoFilter;
// Create cells color for filtering
CellsColor filterColor = workbook.CreateCellsColor();
filterColor.Color = Color.Red;
// Apply fill color filter
filter.AddFillColorFilter(0, BackgroundType.Solid, filterColor, filterColor);
filter.Refresh();
// Save the workbook
workbook.Save("AutoFilterFillColorDemo.xlsx");
}
}
}
```
### See Also
* enum [BackgroundType](../../backgroundtype/)
* class [CellsColor](../../cellscolor/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
