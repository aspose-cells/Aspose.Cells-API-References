##Series.IsVerticalValues
Series property. Indicates whether the data source is vertical
## Series.IsVerticalValues property
Indicates whether the data source is vertical.
```csharp
public bool IsVerticalValues { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyIsVerticalValuesDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
for (int i = 2; i <= 10; i++)
{
worksheet.Cells["A" + i].PutValue("Cat " + (i-1));
worksheet.Cells["B" + i].PutValue(i * 10);
}
// Add chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Add series with vertical values
chart.NSeries.Add("A1:B10", true);
// Demonstrate IsVerticalValues property (read-only)
Console.WriteLine("IsVerticalValues for first series: " + chart.NSeries[0].IsVerticalValues);
// To change orientation, we need to recreate the series with different parameters
chart.NSeries.Clear();
chart.NSeries.Add("A1:B10", false);
Console.WriteLine("IsVerticalValues after recreation: " + chart.NSeries[0].IsVerticalValues);
}
}
}
```
### See Also
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
