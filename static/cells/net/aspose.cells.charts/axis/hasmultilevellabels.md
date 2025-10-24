##Axis.HasMultiLevelLabels
Axis property. Indicates whether the labels shall be shown as multi level
## Axis.HasMultiLevelLabels property
Indicates whether the labels shall be shown as multi level.
```csharp
public bool HasMultiLevelLabels { get; set; }
```
### Remarks
Only valid for category axis.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisPropertyHasMultiLevelLabelsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data with multi-level categories
worksheet.Cells["A1"].PutValue("Main Category");
worksheet.Cells["A2"].PutValue("Fruits");
worksheet.Cells["A3"].PutValue("Vegetables");
worksheet.Cells["B1"].PutValue("Sub Category");
worksheet.Cells["B2"].PutValue("Apple");
worksheet.Cells["B3"].PutValue("Carrot");
worksheet.Cells["C1"].PutValue("Value");
worksheet.Cells["C2"].PutValue(10);
worksheet.Cells["C3"].PutValue(8);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data range including multi-level categories
chart.NSeries.Add("A1:B3", true);
chart.NSeries.CategoryData = "A1:B3";
// Check and display HasMultiLevelLabels property
Console.WriteLine("HasMultiLevelLabels: " + chart.CategoryAxis.HasMultiLevelLabels);
// Save the workbook
workbook.Save("AxisPropertyHasMultiLevelLabelsDemo.xlsx");
}
}
}
```
### See Also
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
