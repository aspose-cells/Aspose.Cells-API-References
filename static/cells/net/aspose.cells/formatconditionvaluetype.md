##Enum FormatConditionValueType
Aspose.Cells.FormatConditionValueType enum. Condition value type
## FormatConditionValueType enumeration
Condition value type.
```csharp
public enum FormatConditionValueType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Formula | `0` | The minimum/ midpoint / maximum value for the gradient is determined by a formula. |
| Max | `1` | Indicates that the maximum value in the range shall be used as the maximum value for the gradient. |
| Min | `2` | Indicates that the minimum value in the range shall be used as the minimum value for the gradient. |
| Number | `3` | Indicates that the minimum / midpoint / maximum value for the gradient is specified by a constant numeric value. |
| Percent | `4` | Value indicates a percentage between the minimum and maximum values in the range shall be used as the minimum / midpoint / maximum value for the gradient. |
| Percentile | `5` | Value indicates a percentile ranking in the range shall be used as the minimum / midpoint / maximum value for the gradient. |
| AutomaticMax | `6` | Indicates that the Automatic maximum value in the range shall be used as the Automatic maximum value for the gradient. |
| AutomaticMin | `7` | Indicates that the Automatic minimum value in the range shall be used as the Automatic minimum value for the gradient. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassFormatConditionValueTypeDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add format conditions
int formatConditionsIndex = sheet.ConditionalFormattings.Add();
FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatConditionsIndex];
int conditionIndex = formatConditions.AddCondition(FormatConditionType.IconSet);
FormatCondition condition = formatConditions[conditionIndex];
// Set icon set properties
condition.IconSet.Type = IconSetType.Boxes5;
condition.IconSet.ShowValue = false;
condition.IconSet.Reverse = true;
// Set cell value and apply formatting
Cell cell = sheet.Cells["A1"];
cell.PutValue("Boxes5 Icon Set Example");
// Access format condition value type
FormatConditionValueType valueType = condition.IconSet.Cfvos[0].Type;
Console.WriteLine("First CFVO Type: " + valueType);
// Display values from the icon set conditions
Console.WriteLine("\nIcon Set Threshold Values:");
foreach (ConditionalFormattingValue cfvo in condition.IconSet.Cfvos)
{
Console.WriteLine($"Type: {cfvo.Type}, Value: {cfvo.Value}");
}
// Save the workbook
workbook.Save("FormatConditionValueTypeDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
