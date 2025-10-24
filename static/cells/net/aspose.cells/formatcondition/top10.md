##FormatCondition.Top10
FormatCondition property. Get the conditional formattings Top10 instance. The default instances rule highlights cells whose values fall in the top 10 bracket. Valid only for type is Top10
## FormatCondition.Top10 property
Get the conditional formatting's "Top10" instance. The default instance's rule highlights cells whose values fall in the top 10 bracket. Valid only for type is Top10.
```csharp
public Top10 Top10 { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class FormatConditionPropertyTop10Demo
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
top10.IsPercent = true;
top10.IsBottom = true;
top10.Rank = 10;
workbook.Save("FormatConditionPropertyTop10Demo.xlsx");
}
}
}
```
### See Also
* class [Top10](../../top10/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
