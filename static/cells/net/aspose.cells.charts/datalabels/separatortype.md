##DataLabels.SeparatorType
DataLabels property. Gets or sets the separator type used for the data labels on a chart
## DataLabels.SeparatorType property
Gets or sets the separator type used for the data labels on a chart.
```csharp
public DataLabelsSeparatorType SeparatorType { get; set; }
```
### Remarks
To set custom separator, please set the property `SeparatorType` as Custom and then specify the expected value for [`SeparatorValue`](../separatorvalue/).
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class DataLabelsPropertySeparatorTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["A2"].PutValue("A");
sheet.Cells["A3"].PutValue("B");
sheet.Cells["A4"].PutValue("C");
sheet.Cells["B1"].PutValue("Value");
sheet.Cells["B2"].PutValue(10);
sheet.Cells["B3"].PutValue(20);
sheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = sheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Enable data labels
chart.NSeries[0].DataLabels.ShowValue = true;
chart.NSeries[0].DataLabels.ShowCategoryName = true;
// Set separator type
chart.NSeries[0].DataLabels.SeparatorType = DataLabelsSeparatorType.Space;
// Save the workbook
workbook.Save("DataLabelsSeparatorTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [DataLabelsSeparatorType](../../datalabelsseparatortype/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
