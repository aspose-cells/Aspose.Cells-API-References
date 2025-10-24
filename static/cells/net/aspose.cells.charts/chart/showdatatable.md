##Chart.ShowDataTable
Chart property. Gets or sets a value indicating whether the chart displays a data table
## Chart.ShowDataTable property
Gets or sets a value indicating whether the chart displays a data table.
```csharp
public bool ShowDataTable { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertyShowDataTableDemo
{
public static void Run()
{
// Create a new Workbook
Workbook workbook = new Workbook();
Worksheet dataSheet = workbook.Worksheets[0];
// Add sample data
dataSheet.Cells["B1"].PutValue("Column 1");
dataSheet.Cells["C1"].PutValue("Column 2");
dataSheet.Cells["A2"].PutValue("Item 1");
dataSheet.Cells["A3"].PutValue("Item 2");
dataSheet.Cells["A4"].PutValue("Item 3");
dataSheet.Cells["B2"].PutValue(10);
dataSheet.Cells["B3"].PutValue(20);
dataSheet.Cells["B4"].PutValue(30);
dataSheet.Cells["C2"].PutValue(15);
dataSheet.Cells["C3"].PutValue(25);
dataSheet.Cells["C4"].PutValue(35);
// Add chart sheet
int chartIndex = workbook.Worksheets.Add(SheetType.Chart);
Worksheet chartSheet = workbook.Worksheets[chartIndex];
// Create chart
chartSheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
Aspose.Cells.Charts.Chart chart = chartSheet.Charts[0];
// Set data source
chart.NSeries.Add("Sheet1!B2:C4", true);
chart.NSeries.CategoryData = "Sheet1!A2:A4";
// Enable data table display
chart.ShowDataTable = true;
// Save the workbook
workbook.Save("ChartWithDataTable.xlsx");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
