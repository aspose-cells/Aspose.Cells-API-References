##FormatCondition.SetFormulas
FormatCondition method. Sets the value or expression associated with this format condition
## FormatCondition.SetFormulas method
Sets the value or expression associated with this format condition.
```csharp
public void SetFormulas(string formula1, string formula2, bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula1 | String | The value or expression associated with this format condition. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| formula2 | String | The value or expression associated with this format condition. The input format is same with formula1 |
| isR1C1 | Boolean | Whether the formula is R1C1 formula. |
| isLocal | Boolean | Whether the formula is locale formatted. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormatConditionMethodSetFormulasWithStringStringBooleanBooleanDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
int formatIndex = cfs.Add();
FormatConditionCollection fcs = cfs[formatIndex];
fcs.AddArea(CellArea.CreateCellArea("A1", "C10"));
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue);
FormatCondition fc = fcs[conditionIndex];
fc.Operator = OperatorType.Between;
fc.SetFormulas("=1", "=2", false, false);
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
