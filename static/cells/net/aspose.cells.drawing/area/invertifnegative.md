##Area.InvertIfNegative
Area property. If the property is true and the value of chart point is a negative number the foreground color and background color will be exchanged
## Area.InvertIfNegative property
If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.
```csharp
public bool InvertIfNegative { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class AreaPropertyInvertIfNegativeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data with negative value
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(-100);
worksheet.Cells["A3"].PutValue(150);
// Add column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add data series and configure area properties
chart.NSeries.Add("A1:A3", true);
chart.NSeries[0].Area.InvertIfNegative = true;
chart.NSeries[0].Area.ForegroundColor = Color.Red;
chart.NSeries[0].Area.BackgroundColor = Color.Yellow;
workbook.Save("AreaPropertyInvertIfNegativeDemo.xls");
}
}
}
```
### See Also
* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
