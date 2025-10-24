##Worksheet.ConvertFormulaReferenceStyle
Worksheet method. Converts the formula reference style
## Worksheet.ConvertFormulaReferenceStyle method
Converts the formula reference style.
```csharp
public string ConvertFormulaReferenceStyle(string formula, bool toR1C1, int baseCellRow,
int baseCellColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The formula to be converted. |
| toR1C1 | Boolean | Which reference style to convert the formula to. If the original formula is of A1 reference style, then this value should be true so the formula will be converted from A1 to R1C1 reference style; If the original formula is of R1C1 reference style, then this value should be false so the formula will be converted from R1C1 to A1 reference style; |
| baseCellRow | Int32 | The row index of the base cell. |
| baseCellColumn | Int32 | The column index of the base cell. |
### Return Value
The converted formula.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodConvertFormulaReferenceStyleWithStringBooleanInt32Int32Demo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Example 1: Convert R1C1 style to A1 style
string formulaR1C1 = "R[0]C23,testDS,R[0]C24";
string formulaA1 = sheet.ConvertFormulaReferenceStyle(formulaR1C1, false, 0, 0);
Console.WriteLine("Converted formula: " + formulaA1);
// Example 2: Convert with mixed references
string formulaMixed = "R[0]C23,testDS,rcurr,R[0]C24";
string convertedMixed = sheet.ConvertFormulaReferenceStyle(formulaMixed, false, 0, 0);
Console.WriteLine("Converted mixed formula: " + convertedMixed);
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
