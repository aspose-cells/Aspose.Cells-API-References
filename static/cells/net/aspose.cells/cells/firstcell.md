##Cells.FirstCell
Cells property. Gets the first cell in this worksheet
## Cells.FirstCell property
Gets the first cell in this worksheet.
```csharp
public Cell FirstCell { get; }
```
### Remarks
Returns null if there is no data in the worksheet.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class CellsPropertyFirstCellDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("Item 1");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["A3"].PutValue("Item 2");
worksheet.Cells["B3"].PutValue(2000);
// Get cells collection
Cells cells = worksheet.Cells;
// Demonstrate FirstCell property
Cell firstCell = cells.FirstCell;
Console.WriteLine($"First cell address: {firstCell.Name}");
Console.WriteLine($"First cell value: {firstCell.Value}");
// Create chart using FirstCell and LastCell
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.SetChartDataRange($"{cells.FirstCell.Name}:{cells.LastCell.Name}", true);
chart.ShowLegend = true;
// Save the workbook
workbook.Save("FirstCellDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
