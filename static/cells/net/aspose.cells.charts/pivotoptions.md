##Class PivotOptions
Aspose.Cells.Charts.PivotOptions class. Represents a complex type that specifies the pivot controls that appear on the chart
## PivotOptions class
Represents a complex type that specifies the pivot controls that appear on the chart
```csharp
public class PivotOptions
```
## Properties
| Name | Description |
| --- | --- |
| [DropZoneCategories](../../aspose.cells.charts/pivotoptions/dropzonecategories/) { get; set; } | Specifies whether a control for each PivotTable field on the PivotTable row axis of the source PivotTable appears on the chart when dropZonesVisible is set to true. |
| [DropZoneData](../../aspose.cells.charts/pivotoptions/dropzonedata/) { get; set; } | Specifies whether a control for each PivotTable field on the PivotTable data axis of the source PivotTable appears on the chart when dropZonesVisible is set to true. |
| [DropZoneFilter](../../aspose.cells.charts/pivotoptions/dropzonefilter/) { get; set; } | Specifies whether a control for each PivotTable field on the PivotTable page axis of the source PivotTable appears on the chart when dropZonesVisible is set to true. |
| [DropZoneSeries](../../aspose.cells.charts/pivotoptions/dropzoneseries/) { get; set; } | Specifies whether a control for each PivotTable field on the PivotTable column axis of the source PivotTable appears on the chart when dropZonesVisible is set to true. |
| [DropZonesVisible](../../aspose.cells.charts/pivotoptions/dropzonesvisible/) { get; set; } | Specifies whether any pivot controls can appear on the pivot chart. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Pivot;
using System;
public class PivotOptionsDemo
{
public static void PivotOptionsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data for the pivot table
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
// Add a pivot table
int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.PivotSource = "PivotTable1";
// Access the PivotOptions of the chart
PivotOptions pivotOptions = chart.PivotOptions;
// Set properties of PivotOptions
pivotOptions.DropZoneFilter = true;
pivotOptions.DropZoneCategories = true;
pivotOptions.DropZoneData = true;
pivotOptions.DropZoneSeries = true;
pivotOptions.DropZonesVisible = true;
// Save the workbook
workbook.Save("PivotOptionsExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
