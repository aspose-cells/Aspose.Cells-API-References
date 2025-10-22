##ChartCollection.Item
ChartCollection property. Gets the Chart element at the specified index
## ChartCollection indexer (1 of 2)
Gets the [`Chart`](../../chart/) element at the specified index.
```csharp
public Chart this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |
### Return Value
The element at the specified index.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
// Access the chart using Item property
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data source and title
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
chart.Title.Text = "Sample Chart";
chart.Title.TextHorizontalAlignment = TextAlignmentType.Center;
// Save the workbook
workbook.Save("output.xlsx");
Console.WriteLine("Chart created successfully with Item property access.");
}
}
}
```
### See Also
* class [Chart](../../chart/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
## ChartCollection indexer (2 of 2)
Gets the chart by the name.
```csharp
public Chart this[string name] { get; }
```
| Parameter | Description |
| --- | --- |
| name | The chart name. |
### Return Value
The chart.
### Remarks
The default chart name is null. So you have to explicitly set the name of the chart.
### See Also
* class [Chart](../../chart/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
