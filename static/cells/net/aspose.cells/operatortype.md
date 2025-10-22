##Enum OperatorType
Aspose.Cells.OperatorType enum. Represents the operator type of conditional format and data validation
## OperatorType enumeration
Represents the operator type of conditional format and data validation.
```csharp
public enum OperatorType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Between | `0` | Represents Between operator of conditional format and data validation. |
| Equal | `1` | Represents Equal operator of conditional format and data validation. |
| GreaterThan | `2` | Represents GreaterThan operator of conditional format and data validation. |
| GreaterOrEqual | `3` | Represents GreaterOrEqual operator of conditional format and data validation. |
| LessThan | `4` | Represents LessThan operator of conditional format and data validation. |
| LessOrEqual | `5` | Represents LessOrEqual operator of conditional format and data validation. |
| None | `6` | Represents no comparison. |
| NotBetween | `7` | Represents NotBetween operator of conditional format and data validation. |
| NotEqual | `8` | Represents NotEqual operator of conditional format and data validation. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class OperatorTypeDemo
{
public static void OperatorTypeExample()
{
// Create a new Workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an empty conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
// Set the conditional format range
CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
fcs.AddArea(ca);
// Add a condition with OperatorType.Between
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A1", "100");
FormatCondition fc = fcs[conditionIndex];
fc.Style.BackgroundColor = System.Drawing.Color.Yellow;
// Add another condition with OperatorType.GreaterThan
int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "50", null);
FormatCondition fc2 = fcs[conditionIndex2];
fc2.Style.BackgroundColor = System.Drawing.Color.Green;
// Save the workbook
workbook.Save("OperatorTypeExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
