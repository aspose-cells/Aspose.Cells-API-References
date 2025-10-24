##CellsHelper.ConvertA1FormulaToR1C1
CellsHelper method. Converts A1 formula of the cell to the r1c1 formula
## CellsHelper.ConvertA1FormulaToR1C1 method
Converts A1 formula of the cell to the r1c1 formula.
```csharp
[Obsolete("Use Worksheet.ConvertFormulaReferenceStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ConvertA1FormulaToR1C1(string formula, int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The A1 formula. |
| row | Int32 | The row index of the cell. |
| column | Int32 | The column index of the cell. |
### Return Value
The R1C1 formula.
### Remarks
NOTE: This member is now obsolete. Instead, please use Worksheet.ConvertFormulaReferenceStyle() method. This property will be removed 12 months later since August 2023. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsHelperMethodConvertA1FormulaToR1C1WithStringInt32Int32Demo
{
public static void Run()
{
// Convert A1 style formula to R1C1 style
string r1c1Formula = CellsHelper.ConvertA1FormulaToR1C1("=A1+B2", 0, 0);
Console.WriteLine("R1C1 Formula: " + r1c1Formula);
}
}
}
```
### See Also
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
