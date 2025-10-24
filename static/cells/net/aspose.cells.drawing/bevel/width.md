##Bevel.Width
Bevel property. Gets and sets the width of the bevel or how far into the shape it is applied. In unit of Points
## Bevel.Width property
Gets and sets the width of the bevel, or how far into the shape it is applied. In unit of Points.
```csharp
public double Width { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class BevelPropertyWidthDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add chart
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 5, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Get first series and set 3D format
Series series = chart.NSeries[0];
Format3D format3D = series.ShapeProperties.Format3D;
// Configure bevel properties with Width demonstration
Bevel topBevel = format3D.TopBevel;
topBevel.Type = BevelPresetType.Circle;
topBevel.Width = 12; // Demonstrating Width property
topBevel.Height = 6;
// Save the workbook
workbook.Save("BevelWidthDemo.xlsx");
}
}
}
```
### See Also
* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
