##Axis.MinorUnit
Axis property. Represents the minor units for the axis
## Axis.MinorUnit property
Represents the minor units for the axis.
```csharp
public double MinorUnit { get; set; }
```
### Remarks
The minor units must be greater than zero.
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisPropertyMinorUnitDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
Cells cells = sheet.Cells;
// Add sample data
cells["A1"].PutValue("Region");
cells["A2"].PutValue("France");
cells["A3"].PutValue("Germany");
cells["A4"].PutValue("England");
cells["B1"].PutValue("Sales");
cells["B2"].PutValue(70000);
cells["B3"].PutValue(55000);
cells["B4"].PutValue(30000);
// Create chart
int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
Chart chart = sheet.Charts[chartIndex];
// Configure chart data
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Configure value axis
chart.ValueAxis.Title.Text = "Sales Amount";
chart.ValueAxis.MajorUnit = 20000;
chart.ValueAxis.MinorUnit = 5000; // Demonstrate MinorUnit property
chart.ValueAxis.MinValue = 0;
chart.ValueAxis.MaxValue = 80000;
// Save the workbook
workbook.Save("AxisPropertyMinorUnitDemo.xlsx");
}
}
}
```
### See Also
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
