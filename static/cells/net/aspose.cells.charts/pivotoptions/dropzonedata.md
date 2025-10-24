##PivotOptions.DropZoneData
PivotOptions property. Specifies whether a control for each PivotTable field on the PivotTable data axis of the source PivotTable appears on the chart when dropZonesVisible is set to true
## PivotOptions.DropZoneData property
Specifies whether a control for each PivotTable field on the PivotTable data axis of the source PivotTable appears on the chart when dropZonesVisible is set to true.
```csharp
public bool DropZoneData { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class PivotOptionsPropertyDropZoneDataDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample data for pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("Books");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["A3"].PutValue("Electronics");
worksheet.Cells["B3"].PutValue(2000);
worksheet.Cells["A4"].PutValue("Books");
worksheet.Cells["B4"].PutValue(1500);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesPivot");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Create chart linked to pivot table
int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.PivotSource = "SalesPivot";
// Configure pivot options with DropZoneData enabled
PivotOptions pivotOptions = chart.PivotOptions;
pivotOptions.DropZoneData = true;
pivotOptions.DropZonesVisible = true;
// Save the result
workbook.Save("PivotOptionsDropZoneDataDemo.xlsx");
}
}
}
```
### See Also
* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
