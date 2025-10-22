##Legend.LegendEntriesLabels
Legend property. Gets the labels of the legend entries after call Chart.Calculate method
## Legend.LegendEntriesLabels property
Gets the labels of the legend entries after call Chart.Calculate() method.
```csharp
[Obsolete("Use Legend.GetLegendLabels method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList LegendEntriesLabels { get; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use Legend.GetLegendLabels method. This property will be removed 12 months later since November 2023. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class LegendPropertyLegendEntriesLabelsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate chart to ensure legend entries are generated
chart.Calculate();
// Get the legend
Legend legend = chart.Legend;
// Display the legend entries labels (using the property)
Console.WriteLine("Legend Entries Labels:");
foreach (string label in legend.LegendEntriesLabels)
{
Console.WriteLine(label);
}
// Save the workbook
workbook.Save("LegendEntriesLabelsDemo.xlsx");
}
}
}
```
### See Also
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
