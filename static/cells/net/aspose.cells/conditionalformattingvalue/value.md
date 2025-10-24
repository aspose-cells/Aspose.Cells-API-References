##ConditionalFormattingValue.Value
ConditionalFormattingValue property. Get or set the value of this conditional formatting value object. It should be used in conjunction with Type
## ConditionalFormattingValue.Value property
Get or set the value of this conditional formatting value object. It should be used in conjunction with Type.
```csharp
public object Value { get; set; }
```
### Remarks
If the value is string and start with "=", it will be processed as a formula, otherwise we will process it as a simple value.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ConditionalFormattingValuePropertyValueDemo
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
FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
// Create icon set conditional formatting
int conditionIndex = fcc.AddCondition(FormatConditionType.IconSet);
FormatCondition condition = fcc[conditionIndex];
condition.IconSet.Type = IconSetType.Arrows3;
// Get the conditional formatting value objects
ConditionalFormattingValueCollection cfvos = condition.IconSet.Cfvos;
// Set values for the icons
cfvos[0].Type = FormatConditionValueType.Min;
cfvos[0].Value = 0;
cfvos[1].Type = FormatConditionValueType.Percent;
cfvos[1].Value = 33;
cfvos[2].Type = FormatConditionValueType.Percent;
cfvos[2].Value = 67;
// Demonstrate Value property usage
Console.WriteLine("First icon value: " + cfvos[0].Value);
Console.WriteLine("Second icon value: " + cfvos[1].Value);
Console.WriteLine("Third icon value: " + cfvos[2].Value);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
