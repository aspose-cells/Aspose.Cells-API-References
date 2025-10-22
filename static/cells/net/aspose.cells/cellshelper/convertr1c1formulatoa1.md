##CellsHelper.ConvertR1C1FormulaToA1
CellsHelper method. Converts the r1c1 formula of the cell to A1 formula
## CellsHelper.ConvertR1C1FormulaToA1 method
Converts the r1c1 formula of the cell to A1 formula.
```csharp
[Obsolete("Use Worksheet.ConvertFormulaReferenceStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ConvertR1C1FormulaToA1(string r1c1Formula, int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| r1c1Formula | String | The r1c1 formula. |
| row | Int32 | The row index of the cell. |
| column | Int32 | The column index of the cell. |
### Return Value
The A1 formula.
### Remarks
NOTE: This member is now obsolete. Instead, please use Worksheet.ConvertFormulaReferenceStyle() method. This property will be removed 12 months later since August 2023. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsHelperMethodConvertR1C1FormulaToA1WithStringInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set R1C1 formulas in cells
worksheet.Cells["A1"].R1C1Formula = "=R[1]C";
worksheet.Cells["B1"].R1C1Formula = "=RC[1]";
worksheet.Cells["A2"].R1C1Formula = "=R2C3";
worksheet.Cells["B2"].R1C1Formula = "=R[-1]C[-1]";
// Convert R1C1 formulas to A1 style
string a1Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["A1"].R1C1Formula, 0, 0);
string b1Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["B1"].R1C1Formula, 0, 0);
string a2Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["A2"].R1C1Formula, 1, 2);
string b2Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["B2"].R1C1Formula, 1, 1);
// Output the results
Console.WriteLine("A1 R1C1: {0} -> A1: {1}", worksheet.Cells["A1"].R1C1Formula, a1Converted);
Console.WriteLine("B1 R1C1: {0} -> A1: {1}", worksheet.Cells["B1"].R1C1Formula, b1Converted);
Console.WriteLine("A2 R1C1: {0} -> A1: {1}", worksheet.Cells["A2"].R1C1Formula, a2Converted);
Console.WriteLine("B2 R1C1: {0} -> A1: {1}", worksheet.Cells["B2"].R1C1Formula, b2Converted);
}
}
}
```
### See Also
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
