##Chart.RefreshPivotData
Chart method. Refreshes charts data from pivot table
## Chart.RefreshPivotData method
Refreshes chart's data from pivot table.
```csharp
public void RefreshPivotData()
```
### Remarks
We will gather data from pivot data source to the pivot table report. This method is only used to gather all data to a pivot chart.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartMethodRefreshPivotDataDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add sample data to the first worksheet
Worksheet dataSheet = workbook.Worksheets[0];
dataSheet.Cells["A1"].PutValue("Product");
dataSheet.Cells["B1"].PutValue("Sales");
dataSheet.Cells["A2"].PutValue("A");
dataSheet.Cells["B2"].PutValue(100);
dataSheet.Cells["A3"].PutValue("B");
dataSheet.Cells["B3"].PutValue(200);
dataSheet.Cells["A4"].PutValue("C");
dataSheet.Cells["B4"].PutValue(300);
// Create a pivot table
Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
pivotSheet.PivotTables.Add("A1", dataSheet.Cells["A1:B4"].Name, "PivotTable1");
// Add a chart
int chartIndex = pivotSheet.Charts.Add(ChartType.Column, 5, 0, 15, 8);
Aspose.Cells.Charts.Chart chart = pivotSheet.Charts[chartIndex];
// Set pivot chart data source
chart.PivotSource = "Pivot!PivotTable1";
// Refresh pivot data in the chart
chart.RefreshPivotData();
// Save the workbook
workbook.Save("PivotChartWithRefresh.xlsx");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
