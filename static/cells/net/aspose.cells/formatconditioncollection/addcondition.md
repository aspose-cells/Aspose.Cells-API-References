##FormatConditionCollection.AddCondition
FormatConditionCollection method. Adds a formatting condition
## AddCondition(FormatConditionType, OperatorType, string, string) {#addcondition_1}
Adds a formatting condition.
```csharp
public int AddCondition(FormatConditionType type, OperatorType operatorType, string formula1,
string formula2)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | FormatConditionType | The type of format condition. |
| operatorType | OperatorType | The operator type |
| formula1 | String | The value or expression associated with conditional formatting. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| formula2 | String | The value or expression associated with conditional formatting. The input format is same with formula1 |
### Return Value
Formatting condition object index;
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormatConditionCollectionMethodAddConditionWithFormatConditionTypeOperatorTypDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 10;
ca.StartColumn = 0;
ca.EndColumn = 10;
fcs.AddArea(ca);
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "-50", "-1");
FormatCondition fc = fcs[conditionIndex];
fc.Style.Font.Color = Color.Red;
conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "0", "50");
fc = fcs[conditionIndex];
fc.Style.Font.Color = Color.Green;
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* enum [FormatConditionType](../../formatconditiontype/)
* enum [OperatorType](../../operatortype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## AddCondition(FormatConditionType) {#addcondition}
Add a format condition.
```csharp
public int AddCondition(FormatConditionType type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | FormatConditionType | Format condition type. |
### Return Value
Formatting condition object index;
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormatConditionCollectionMethodAddConditionWithFormatConditionTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create format conditions
int formatIndex = worksheet.ConditionalFormattings.Add();
FormatConditionCollection conditions = worksheet.ConditionalFormattings[formatIndex];
// Add range
CellArea area = new CellArea
{
StartRow = 0,
StartColumn = 0,
EndRow = 5,
EndColumn = 5
};
conditions.AddArea(area);
// Add conditions (returns int index)
conditions.AddCondition(FormatConditionType.ColorScale);
conditions.AddCondition(FormatConditionType.IconSet);
conditions.AddCondition(FormatConditionType.DataBar);
workbook.Save("ConditionalFormattingDemo.xlsx");
}
}
}
```
### See Also
* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
