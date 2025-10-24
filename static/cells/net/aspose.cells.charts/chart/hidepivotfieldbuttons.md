##Chart.HidePivotFieldButtons
Chart property. Indicates whether hide the pivot chart field buttons only when the chart is PivotChart
## Chart.HidePivotFieldButtons property
Indicates whether hide the pivot chart field buttons only when the chart is PivotChart.
```csharp
public bool HidePivotFieldButtons { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class ChartPropertyHidePivotFieldButtonsDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 100;
worksheet.Cells["B3"].Value = 150;
worksheet.Cells["B4"].Value = 200;
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Create chart
int chartIndex = worksheet.Charts.Add(ChartType.Column3DClustered, 9, 6, 24, 14);
Chart chart = worksheet.Charts[chartIndex];
chart.PivotSource = "Sheet1!PivotTable1";
// Demonstrate HidePivotFieldButtons property
chart.HidePivotFieldButtons = false; // Show pivot field buttons
chart.RefreshPivotData();
// Save the workbook
workbook.Save("HidePivotFieldButtonsDemo.xlsx");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
