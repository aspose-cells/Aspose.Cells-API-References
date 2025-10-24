##AutoFilter.AddFontColorFilter
AutoFilter method. Adds a font color filter
## AutoFilter.AddFontColorFilter method
Adds a font color filter.
```csharp
public void AddFontColorFilter(int fieldIndex, CellsColor color)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| color | CellsColor | The [`CellsColor`](../../cellscolor/) object. |
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFilterMethodAddFontColorFilterWithInt32CellsColorDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data with different font colors
Cells cells = worksheet.Cells;
cells["A1"].PutValue("Header");
cells["A2"].PutValue("Item 1");
cells["A3"].PutValue("Item 2");
cells["A4"].PutValue("Item 3");
// Set font colors
Style style = cells["A2"].GetStyle();
style.Font.Color = Color.Red;
cells["A2"].SetStyle(style);
style = cells["A3"].GetStyle();
style.Font.Color = Color.Blue;
cells["A3"].SetStyle(style);
style = cells["A4"].GetStyle();
style.Font.Color = Color.Green;
cells["A4"].SetStyle(style);
// Apply auto filter
worksheet.AutoFilter.Range = "A1:A4";
AutoFilter filter = worksheet.AutoFilter;
// Create color filter for red font
CellsColor cr = workbook.CreateCellsColor();
cr.Color = Color.Red;
// Add font color filter
filter.AddFontColorFilter(0, cr);
filter.Refresh();
// Save the workbook
workbook.Save("AutoFilterFontColorDemo.xlsx");
}
}
}
```
### See Also
* class [CellsColor](../../cellscolor/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
