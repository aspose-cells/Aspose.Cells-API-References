##Chart.PivotSource
Chart property. The source is the data of the pivotTable. If PivotSource is not empty the chart is PivotChart
## Chart.PivotSource property
The source is the data of the pivotTable. If PivotSource is not empty ,the chart is PivotChart.
```csharp
public string PivotSource { get; set; }
```
### Remarks
If the pivot table "PivotTable1" in the Worksheet "Sheet1" in the file "Book1.xls". The pivotSource could be "[Book1.xls]Sheet1!PivotTable1" if the chart and the PivotTable is not in the same workbook. If you set this property ,the previous data source setting will be lost.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertyPivotSourceDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
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
// Add pivot table
int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Add chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set pivot source for the chart
chart.PivotSource = "Sheet1!PivotTable1";
// Refresh pivot data and chart
pivotTable.RefreshData();
pivotTable.CalculateData();
chart.RefreshPivotData();
// Save the workbook
workbook.Save("PivotSourceDemo.xlsx", SaveFormat.Xlsx);
Console.WriteLine("Chart PivotSource demo executed successfully.");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
