##ChartTextFrame.LinkedSource
ChartTextFrame property. Gets and sets a reference to the worksheet
## ChartTextFrame.LinkedSource property
Gets and sets a reference to the worksheet.
```csharp
public virtual string LinkedSource { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartTextFramePropertyLinkedSourceDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["P1"].PutValue("Chart Title");
// Add chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart title and link it to cell P1
chart.Title.Text = "Linked Title";
chart.Title.LinkedSource = "='" + worksheet.Name + "'!$P$1";
// Save the workbook
workbook.Save("output.xlsx");
// Verify the linked source
Console.WriteLine("Chart Title Linked Source: " + chart.Title.LinkedSource);
}
}
}
```
### See Also
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
