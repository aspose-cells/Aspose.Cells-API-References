##FormatCondition.Priority
FormatCondition property. The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and rendered. Lower numeric values are higher priority than higher numeric values where 1 is the highest priority
## FormatCondition.Priority property
The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and rendered. Lower numeric values are higher priority than higher numeric values, where '1' is the highest priority.
```csharp
public int Priority { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormatConditionPropertyPriorityDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
for (int i = 0; i < 10; i++)
{
sheet.Cells[i, 0].PutValue(i + 1);
}
// Add conditional formatting
int formatIndex = sheet.ConditionalFormattings.Add();
FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatIndex];
// Add conditions
int conditionIndex1 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "2", "5");
int conditionIndex2 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "6", "9");
// Set priorities
formatConditions[conditionIndex1].Priority = 2;
formatConditions[conditionIndex2].Priority = 1;
// Demonstrate Priority property usage
Console.WriteLine("Condition 1 Priority: " + formatConditions[conditionIndex1].Priority);
Console.WriteLine("Condition 2 Priority: " + formatConditions[conditionIndex2].Priority);
// Save the workbook
workbook.Save("ConditionalFormattingPriorityDemo.xlsx");
}
}
}
```
### See Also
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
