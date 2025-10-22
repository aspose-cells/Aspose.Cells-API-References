##Axis.CustUnit
Axis property. Specifies a custom value for the display unit
## Axis.CustUnit property
Specifies a custom value for the display unit.
```csharp
[Obsolete("Use Axis.CustomUnit property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CustUnit { get; set; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use Axis.CustomUnit property. This property will be removed 12 months later since January 2023. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class AxisPropertyCustUnitDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["A5"].PutValue("D");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(1000000);
worksheet.Cells["B3"].PutValue(2000000);
worksheet.Cells["B4"].PutValue(3000000);
worksheet.Cells["B5"].PutValue(4000000);
// Add a chart and set its data range
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B5", true);
chart.NSeries.CategoryData = "A2:A5";
// Get the value axis
Axis valueAxis = chart.ValueAxis;
// Display current CustUnit value (obsolete property)
Console.WriteLine("Current CustUnit value: " + valueAxis.CustUnit);
// Set a new custom unit value (1,000,000)
valueAxis.CustUnit = 1000000;
valueAxis.IsDisplayUnitLabelShown = true;
// Display the new CustUnit value
Console.WriteLine("New CustUnit value: " + valueAxis.CustUnit);
// Save the result
workbook.Save("AxisPropertyCustUnitDemo.xlsx");
}
}
}
```
### See Also
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
