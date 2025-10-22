##Bevel.Height
Bevel property. Gets and sets the height of the bevel or how far above the shape it is applied. In unit of Points
## Bevel.Height property
Gets and sets the height of the bevel, or how far above the shape it is applied. In unit of Points.
```csharp
public double Height { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class BevelPropertyHeightDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["A2"].PutValue("Product A");
worksheet.Cells["A3"].PutValue("Product B");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["B3"].PutValue(1500);
// Add a 3D column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B3", true);
// Access the plot area's 3D format
Format3D format3D = chart.PlotArea.ShapeProperties.Format3D;
// Configure top bevel with Height property
Bevel topBevel = format3D.TopBevel;
topBevel.Type = BevelPresetType.ArtDeco;
topBevel.Width = 8;
topBevel.Height = 4.5; // Demonstrating Height property usage
// Save the workbook
workbook.Save("BevelHeightDemo.xlsx");
}
}
}
```
### See Also
* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
