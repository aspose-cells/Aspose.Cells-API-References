##Top10.IsPercent
Top10 property. Get or set whether a top/bottom n rule is a top/bottom n percent rule. Default value is false
## Top10.IsPercent property
Get or set whether a "top/bottom n" rule is a "top/bottom n percent" rule. Default value is false.
```csharp
public bool IsPercent { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class Top10PropertyIsPercentDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
for (int i = 0; i < 10; i++)
{
worksheet.Cells[i, 0].PutValue(i + 1);
}
// Add a Top10 conditional formatting rule
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
fcc.AddCondition(FormatConditionType.Top10, OperatorType.None, null, null);
// Get the Top10 format condition
FormatCondition fc = fcc[0];
// Set Top10 properties
fc.Top10.IsPercent = true;  // Demonstrate IsPercent property
fc.Top10.IsBottom = false;
fc.Top10.Rank = 3;
// Apply formatting style
Style style = workbook.CreateStyle();
style.Font.Color = System.Drawing.Color.Red;
fc.Style = style;
// Save the workbook
workbook.Save("Top10IsPercentDemo.xlsx");
}
}
}
```
### See Also
* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
