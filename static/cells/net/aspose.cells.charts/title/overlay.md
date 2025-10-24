##Title.OverLay
Title property. Represents overlay centered title on chart without resizing chart
## Title.OverLay property
Represents overlay centered title on chart without resizing chart.
```csharp
public bool OverLay { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class TitlePropertyOverLayDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 1].PutValue("Income");
cells[1, 0].PutValue("Company A");
cells[2, 0].PutValue("Company B");
cells[3, 0].PutValue("Company C");
cells[1, 1].PutValue(10000);
cells[2, 1].PutValue(20000);
cells[3, 1].PutValue(30000);
int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 9, 9, 21, 15);
Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
chart.Title.Text = "Income Analysis";
chart.Title.OverLay = true; // Demonstrating OverLay property
workbook.Save("TitleOverlayDemo.xlsx");
}
}
}
```
### See Also
* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
