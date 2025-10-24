##PivotTableCalculateOption.RefreshCharts
PivotTableCalculateOption property. Indicates whether refreshing charts are based on this pivot table
## PivotTableCalculateOption.RefreshCharts property
Indicates whether refreshing charts are based on this pivot table.
```csharp
public bool RefreshCharts { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableCalculateOptionPropertyRefreshChartsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Banana");
worksheet.Cells["A4"].PutValue("Orange");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(150);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["B4"].PutValue(180);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesPivot");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Create a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.PivotSource = "SalesPivot";
chart.SetChartDataRange("D1:E4", true);
// Calculate with RefreshCharts option
PivotTableCalculateOption options = new PivotTableCalculateOption
{
RefreshData = true,
RefreshCharts = true
};
pivotTable.CalculateData(options);
workbook.Save("PivotTableRefreshChartsDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTableCalculateOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
