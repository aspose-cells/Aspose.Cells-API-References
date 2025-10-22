##Axis.MinValue
Axis property. Represents the minimum value on the value axis
## Axis.MinValue property
Represents the minimum value on the value axis.
```csharp
public object MinValue { get; set; }
```
### Remarks
The minValue type only can be double or DateTime
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisPropertyMinValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet and add sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["B1"].PutValue(40);
worksheet.Cells["B2"].PutValue(50);
worksheet.Cells["B3"].PutValue(60);
// Add a chart and set data range
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B3", false);
// Configure value axis properties
chart.ValueAxis.MinValue = 15;  // Setting minimum value
chart.ValueAxis.MaxValue = 70;
chart.ValueAxis.MajorUnit = 10;
// Save the workbook
workbook.Save("AxisMinValueDemo.xlsx");
Console.WriteLine("Chart created with MinValue set to 15.");
}
}
}
```
### See Also
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
