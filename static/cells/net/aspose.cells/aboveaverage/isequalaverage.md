##AboveAverage.IsEqualAverage
AboveAverage property. Get or set the flag indicating whether the aboveAverage and belowAverage criteria is inclusive of the average itself or exclusive of that value. true indicates to include the average value in the criteria. Default value is false
## AboveAverage.IsEqualAverage property
Get or set the flag indicating whether the 'aboveAverage' and 'belowAverage' criteria is inclusive of the average itself, or exclusive of that value. 'true' indicates to include the average value in the criteria. Default value is false.
```csharp
public bool IsEqualAverage { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class AboveAveragePropertyIsEqualAverageDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
CellArea ca = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };
fcs.AddArea(ca);
int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
FormatCondition fc = fcs[conditionIndex];
fc.Style.BackgroundColor = Color.LightBlue;
// Demonstrate IsEqualAverage property
fc.AboveAverage.IsAboveAverage = true;
fc.AboveAverage.IsEqualAverage = false; // Cells equal to average won't be formatted
// Populate sample data
worksheet.Cells["A1"].Value = 10;
worksheet.Cells["A2"].Value = 20;
worksheet.Cells["A3"].Value = 30;
worksheet.Cells["A4"].Value = 40;
worksheet.Cells["A5"].Value = 50; // Average is 30
workbook.Save("AboveAverageIsEqualAverageDemo.xlsx");
}
}
}
```
### See Also
* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
