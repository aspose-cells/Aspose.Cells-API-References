##FormatCondition.StopIfTrue
FormatCondition property. True no rules with lower priority may be applied over this rule when this rule evaluates to true. Only applies for Excel 2007
## FormatCondition.StopIfTrue property
True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. Only applies for Excel 2007;
```csharp
public bool StopIfTrue { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormatConditionPropertyStopIfTrueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["A4"].PutValue(40);
// Add conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
// Add condition and set StopIfTrue
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "15", "35");
FormatCondition condition = fcs[conditionIndex];
condition.StopIfTrue = true;
// Add another condition that would normally override the first
int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "25", "");
FormatCondition condition2 = fcs[conditionIndex2];
condition2.StopIfTrue = false;
// Save the workbook
workbook.Save("StopIfTrueDemo.xlsx");
}
}
}
```
### See Also
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
