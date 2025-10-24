##Cell.IsArrayFormula
Cell property. Indicates whether the cell formula is an array formula
## Cell.IsArrayFormula property
Indicates whether the cell formula is an array formula.
```csharp
public bool IsArrayFormula { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyIsArrayFormulaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create an array formula in cell B2
worksheet.Cells["B2"].SetArrayFormula("SUM(A1:A10*B1:B10)", 1, 1);
// Check if the cell contains an array formula
bool isArrayFormula = worksheet.Cells["B2"].IsArrayFormula;
// Output the result
Console.WriteLine("Cell B2 is an array formula: " + isArrayFormula);
// Save the workbook
workbook.Save("IsArrayFormulaDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
