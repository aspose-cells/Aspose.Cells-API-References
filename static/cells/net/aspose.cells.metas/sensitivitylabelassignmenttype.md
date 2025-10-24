##Enum SensitivityLabelAssignmentType
Aspose.Cells.Metas.SensitivityLabelAssignmentType enum. Represents the assignment method for the sensitivity label
## SensitivityLabelAssignmentType enumeration
Represents the assignment method for the sensitivity label.
```csharp
public enum SensitivityLabelAssignmentType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Standard | `0` | Use for any sensitivity label that was not directly applied by the user. |
| Privileged | `1` | Use for any sensitivity label that was directly applied by the user. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Metas;
public class MetasClassSensitivityLabelAssignmentTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Demonstrate SensitivityLabelAssignmentType enum values
SensitivityLabelAssignmentType standardAssignment = SensitivityLabelAssignmentType.Standard;
SensitivityLabelAssignmentType privilegedAssignment = SensitivityLabelAssignmentType.Privileged;
// Apply sensitivity label assignment type to worksheet metadata
worksheet.Cells["A1"].PutValue("Standard Sensitivity Label Assignment:");
worksheet.Cells["B1"].PutValue(standardAssignment.ToString());
worksheet.Cells["A2"].PutValue("Privileged Sensitivity Label Assignment:");
worksheet.Cells["B2"].PutValue(privilegedAssignment.ToString());
// Conditional formatting based on sensitivity label assignment type
int standardLabelIndex = (int)SensitivityLabelAssignmentType.Standard;
int privilegedLabelIndex = (int)SensitivityLabelAssignmentType.Privileged;
FormatConditionCollection formatConditions = worksheet.ConditionalFormattings[0];
CellArea cellArea = new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 1 };
int index = formatConditions.AddCondition(FormatConditionType.Expression, OperatorType.None, "", "");
FormatCondition formatCondition = formatConditions[index];
formatCondition.SetFormulas("=$B$1=\"" + standardAssignment.ToString() + "\"", "", false, false);
formatCondition.Type = FormatConditionType.Expression;
formatCondition.Style.BackgroundColor = System.Drawing.Color.LightBlue;
index = formatConditions.AddCondition(FormatConditionType.Expression, OperatorType.None, "", "");
formatCondition = formatConditions[index];
formatCondition.SetFormulas("=$B$2=\"" + privilegedAssignment.ToString() + "\"", "", false, false);
formatCondition.Type = FormatConditionType.Expression;
formatCondition.Style.BackgroundColor = System.Drawing.Color.LightGreen;
// Save the workbook
workbook.Save("SensitivityLabelAssignmentTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)
