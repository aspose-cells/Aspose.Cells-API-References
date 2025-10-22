##Series.CountOfDataValues
Series property. Gets the number of the data values
## Series.CountOfDataValues property
Gets the number of the data values.
```csharp
public int CountOfDataValues { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyCountOfDataValuesDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
for (int i = 0; i < 4; i++)
{
worksheet.Cells[i, 0].PutValue(i + 1); // A1:A4 with values 1-4
}
// Create a chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add series using the data range
chart.NSeries.Add("A1:A4", true);
// Display the count of data values in the first series
Console.WriteLine("Count of data values in series: " + chart.NSeries[0].CountOfDataValues);
// Save the workbook
workbook.Save("SeriesPropertyCountOfDataValuesDemo.xlsx");
}
}
}
```
### See Also
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
