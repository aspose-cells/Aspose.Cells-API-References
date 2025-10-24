##AboveAverage.StdDev
AboveAverage property. Get or set the number of standard deviations to include above or below the average in the conditional formatting rule. The input value must between 0 and 3 include 0 and 3. Setting this value to 0 means stdDev is not set. The default value is 0
## AboveAverage.StdDev property
Get or set the number of standard deviations to include above or below the average in the conditional formatting rule. The input value must between 0 and 3 (include 0 and 3). Setting this value to 0 means stdDev is not set. The default value is 0.
```csharp
public int StdDev { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class AboveAveragePropertyStdDevDemo
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
fc.Style.BackgroundColor = Color.Yellow;
fc.AboveAverage.IsAboveAverage = true;
fc.AboveAverage.StdDev = 2;
// Populate sample data
worksheet.Cells["A1"].Value = 10;
worksheet.Cells["A2"].Value = 20;
worksheet.Cells["A3"].Value = 30;
worksheet.Cells["A4"].Value = 40;
worksheet.Cells["A5"].Value = 50;
workbook.Save("AboveAverageStdDevDemo.xlsx");
}
}
}
```
### See Also
* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
