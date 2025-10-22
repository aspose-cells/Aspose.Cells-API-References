##PivotOptions.DropZonesVisible
PivotOptions property. Specifies whether any pivot controls can appear on the pivot chart
## PivotOptions.DropZonesVisible property
Specifies whether any pivot controls can appear on the pivot chart.
```csharp
public bool DropZonesVisible { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotOptionsPropertyDropZonesVisibleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample data for pivot table
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["A4"].PutValue("A");
worksheet.Cells["B4"].PutValue(30);
worksheet.Cells["A5"].PutValue("B");
worksheet.Cells["B5"].PutValue(40);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Create chart linked to pivot table
int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.PivotSource = "PivotTable1";
// Configure pivot options with DropZonesVisible
PivotOptions pivotOptions = chart.PivotOptions;
pivotOptions.DropZonesVisible = true;
workbook.Save("PivotOptionsDropZonesVisibleDemo.xlsx");
}
}
}
```
### See Also
* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
