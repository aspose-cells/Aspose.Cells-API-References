##Top10.Rank
Top10 property. Get or set the value of n in a top/bottom n conditional formatting rule. If IsPercent is true the value must between 0 and 100. Otherwise it must between 0 and 1000. Default value is 10
## Top10.Rank property
Get or set the value of "n" in a "top/bottom n" conditional formatting rule. If IsPercent is true, the value must between 0 and 100. Otherwise it must between 0 and 1000. Default value is 10.
```csharp
public int Rank { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class Top10PropertyRankDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
fcs.AddArea(ca);
int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
FormatCondition fc = fcs[conditionIndex];
fc.Style.BackgroundColor = Color.Red;
Top10 top10 = fc.Top10;
top10.Rank = 5;
workbook.Save("Top10RankExample.xlsx");
}
}
}
```
### See Also
* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
