##ConditionalFormattingValueCollection.Add
ConditionalFormattingValueCollection method. Adds ConditionalFormattingValue object
## ConditionalFormattingValueCollection.Add method
Adds [`ConditionalFormattingValue`](../../conditionalformattingvalue/) object.
```csharp
public int Add(FormatConditionValueType type, string value)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | FormatConditionValueType | The value type. |
| value | String | The value. |
### Return Value
Returns the index of new object in the list.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ConditionalFormattingValueCollectionMethodAddWithFormatConditionValueTypeStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
CellArea ca = new CellArea
{
StartRow = 0,
EndRow = 2,
StartColumn = 0,
EndColumn = 0
};
fcs.AddArea(ca);
int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
FormatCondition cond = fcs[conditionIndex];
IconSet iconSet = cond.IconSet;
iconSet.Type = IconSetType.Arrows3;
ConditionalFormattingValueCollection cfvos = iconSet.Cfvos;
int cfvIndex = cfvos.Add(FormatConditionValueType.Number, "50");
sheet.Cells["A1"].PutValue(10);
sheet.Cells["A2"].PutValue(120);
sheet.Cells["A3"].PutValue(260);
workbook.Save("ConditionalFormattingValueCollectionExample.xlsx");
}
}
}
```
### See Also
* enum [FormatConditionValueType](../../formatconditionvaluetype/)
* class [ConditionalFormattingValueCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
