##Format3D.HasTopBevelData
Format3D method. Indicates if the shape has top bevel data
## Format3D.HasTopBevelData method
Indicates if the shape has top bevel data.
```csharp
public bool HasTopBevelData()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class Format3DMethodHasTopBevelDataDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue(10);
sheet.Cells["A2"].PutValue(20);
sheet.Cells["A3"].PutValue(30);
// Create 3D chart
int chartIndex = sheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 8);
Chart chart = sheet.Charts[chartIndex];
chart.NSeries.Add("A1:A3", true);
// Get 3D format
Format3D format3D = chart.NSeries[0].ShapeProperties.Format3D;
// Set top bevel
format3D.TopBevel.Type = BevelPresetType.Circle;
format3D.TopBevel.Width = 6;
format3D.TopBevel.Height = 6;
// Check and display bevel data
if (format3D.HasTopBevelData())
{
Console.WriteLine("Top Bevel Type: " + format3D.TopBevel.Type);
Console.WriteLine("Top Bevel Width: " + format3D.TopBevel.Width);
Console.WriteLine("Top Bevel Height: " + format3D.TopBevel.Height);
}
workbook.Save("Format3DTopBevelDemo.xlsx");
}
}
}
```
### See Also
* class [Format3D](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
