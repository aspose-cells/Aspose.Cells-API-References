##LegendEntry.AutoScaleFont
LegendEntry property. True if the text in the object changes font size when the object size changes. The default value is True
## LegendEntry.AutoScaleFont property
True if the text in the object changes font size when the object size changes. The default value is True.
```csharp
public bool AutoScaleFont { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class LegendEntryPropertyAutoScaleFontDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].PutValue("Product");
sheet.Cells["A2"].PutValue("Widget A");
sheet.Cells["A3"].PutValue("Widget B");
sheet.Cells["B1"].PutValue("Sales");
sheet.Cells["B2"].PutValue(1500);
sheet.Cells["B3"].PutValue(3000);
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 5, 15, 10);
Chart chart = sheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B3", true);
LegendEntry firstEntry = chart.Legend.LegendEntries[0];
firstEntry.AutoScaleFont = true;
firstEntry.Font.Size = 14;
workbook.Save("LegendEntryAutoScaleFontDemo.xlsx");
}
}
}
```
### See Also
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
