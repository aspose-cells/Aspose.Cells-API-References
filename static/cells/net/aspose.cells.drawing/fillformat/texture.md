##FillFormat.Texture
FillFormat property. Represents the texture type for the specified fill
## FillFormat.Texture property
Represents the texture type for the specified fill.
```csharp
public TextureType Texture { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class FillFormatPropertyTextureDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for chart
sheet.Cells["A1"].PutValue("Item");
sheet.Cells["A2"].PutValue("Product A");
sheet.Cells["A3"].PutValue("Product B");
sheet.Cells["A4"].PutValue("Product C");
sheet.Cells["B1"].PutValue("Sales");
sheet.Cells["B2"].PutValue(1000);
sheet.Cells["B3"].PutValue(2000);
sheet.Cells["B4"].PutValue(3000);
// Add a chart
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = sheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Set texture for the first series' third point
ChartPoint point = chart.NSeries[0].Points[2];
point.Area.FillFormat.Texture = TextureType.Oak;
// Save the workbook
workbook.Save("FillFormatTextureDemo.xlsx");
}
}
}
```
### See Also
* enum [TextureType](../../texturetype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
