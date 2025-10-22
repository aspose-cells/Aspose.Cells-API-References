##PivotOptions.DropZoneCategories
PivotOptions property. Specifies whether a control for each PivotTable field on the PivotTable row axis of the source PivotTable appears on the chart when dropZonesVisible is set to true
## PivotOptions.DropZoneCategories property
Specifies whether a control for each PivotTable field on the PivotTable row axis of the source PivotTable appears on the chart when dropZonesVisible is set to true.
```csharp
public bool DropZoneCategories { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class PivotOptionsPropertyDropZoneCategoriesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet and some sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
// Add a chart that uses pivot data
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Access pivot options from the chart
PivotOptions options = chart.PivotOptions;
// Demonstrate DropZoneCategories property
options.DropZoneCategories = true;
Console.WriteLine("DropZoneCategories enabled: " + options.DropZoneCategories);
// Save the workbook
workbook.Save("PivotOptionsDemo.xlsx");
}
}
}
```
### See Also
* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
