##ColorScale.MidCfvo
ColorScale property. Get or set this ColorScales mid value object. Cannot set CFValueObject with type FormatConditionValueType.Max or FormatConditionValueType.Min to it
## ColorScale.MidCfvo property
Get or set this ColorScale's mid value object. Cannot set CFValueObject with type FormatConditionValueType.Max or FormatConditionValueType.Min to it.
```csharp
public ConditionalFormattingValue MidCfvo { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ColorScalePropertyMidCfvoDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add some sample data
for (int i = 0; i < 10; i++)
{
sheet.Cells[i, 0].PutValue(i * 10);
}
// Add a color scale conditional formatting
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
int conditionIndex = fcc.AddCondition(FormatConditionType.ColorScale);
// Set the mid point value for the color scale
ColorScale colorScale = fcc[conditionIndex].ColorScale;
colorScale.MidCfvo.Type = FormatConditionValueType.Number;
colorScale.MidCfvo.Value = 50;
// Save the workbook
workbook.Save("ColorScalePropertyMidCfvoDemo.xlsx");
}
}
}
```
### See Also
* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
