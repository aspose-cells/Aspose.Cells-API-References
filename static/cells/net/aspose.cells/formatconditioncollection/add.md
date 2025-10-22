##FormatConditionCollection.Add
FormatConditionCollection method. Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three conditional formats. References to the other sheets are not allowed in the formulas of conditional formatting
## FormatConditionCollection.Add method
Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three conditional formats. References to the other sheets are not allowed in the formulas of conditional formatting.
```csharp
public int[] Add(CellArea cellArea, FormatConditionType type, OperatorType operatorType,
string formula1, string formula2)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | Conditional formatted cell range. |
| type | FormatConditionType | Type of conditional formatting.It could be one of the members of FormatConditionType. |
| operatorType | OperatorType | Comparison operator.It could be one of the members of OperatorType. |
| formula1 | String | The value or expression associated with conditional formatting. |
| formula2 | String | The value or expression associated with conditional formatting |
### Return Value
[0]:Formatting condition object index;[1] Effected cell rang index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormatConditionCollectionMethodAddWithCellAreaFormatConditionTypeOpeDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
Cells cells = sheet.Cells;
// Populate sample data
for (int i = 0; i < 5; i++)
{
cells[i, 0].PutValue(i);
}
// Add conditional formatting
ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
FormatConditionCollection fcc = cfc[cfc.Add()];
// Demonstrate Add method with specified parameters
fcc.Add(
CellArea.CreateCellArea(0, 0, 4, 0),
FormatConditionType.Expression,
OperatorType.None,
"=A1>AVERAGE(OFFSET($A$1:$A$5,0,0)-0)",
null
);
// Apply formatting
int fontSize = wb.DefaultStyle.Font.Size;
fcc[0].Style.Font.Size = fontSize + 2;
// Save the workbook to demonstrate the result
wb.Save("ConditionalFormattingDemo.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* enum [FormatConditionType](../../formatconditiontype/)
* enum [OperatorType](../../operatortype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
