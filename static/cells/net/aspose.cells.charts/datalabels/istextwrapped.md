##DataLabels.IsTextWrapped
DataLabels property. Gets or sets a value indicating whether the text is wrapped
## DataLabels.IsTextWrapped property
Gets or sets a value indicating whether the text is wrapped.
```csharp
public override bool IsTextWrapped { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class DataLabelsPropertyIsTextWrappedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["A4"].PutValue("Banana");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(120);
worksheet.Cells["B3"].PutValue(85);
worksheet.Cells["B4"].PutValue(65);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access data labels
Aspose.Cells.Charts.DataLabels labels = chart.NSeries[0].DataLabels;
// Show data labels
labels.ShowValue = true;
// Demonstrate IsTextWrapped property
Console.WriteLine("Before setting IsTextWrapped: " + labels.IsTextWrapped);
labels.IsTextWrapped = true;
Console.WriteLine("After setting IsTextWrapped: " + labels.IsTextWrapped);
// Save the workbook
workbook.Save("DataLabels_IsTextWrapped_Demo.xlsx");
}
}
}
```
### See Also
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
