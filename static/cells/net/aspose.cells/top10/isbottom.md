##Top10.IsBottom
Top10 property. Get or set whether a top/bottom n rule is a bottom n rule. Default value is false
## Top10.IsBottom property
Get or set whether a "top/bottom n" rule is a "bottom n" rule. Default value is false.
```csharp
public bool IsBottom { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class Top10PropertyIsBottomDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
for (int i = 0; i < 10; i++)
{
sheet.Cells[i, 0].PutValue(i + 1);
}
// Add conditional formatting
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
fcs.AddArea(new CellArea { StartRow = 0, EndRow = 9, StartColumn = 0, EndColumn = 0 });
// Add Top10 condition
int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
FormatCondition fc = fcs[conditionIndex];
fc.Style.BackgroundColor = Color.Red;
// Configure Top10 properties
Top10 top10 = fc.Top10;
top10.IsBottom = true; // Highlight bottom values
top10.IsPercent = false;
top10.Rank = 3; // Highlight bottom 3 values
workbook.Save("Top10IsBottomExample.xlsx");
}
}
}
```
### See Also
* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
