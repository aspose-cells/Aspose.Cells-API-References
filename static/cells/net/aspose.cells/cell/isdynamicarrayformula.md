##Cell.IsDynamicArrayFormula
Cell property. Indicates whether the cells formula is dynamic array formulatrue or legacy array formulafalse
## Cell.IsDynamicArrayFormula property
Indicates whether the cell's formula is dynamic array formula(true) or legacy array formula(false).
```csharp
public bool IsDynamicArrayFormula { get; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyIsDynamicArrayFormulaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set a dynamic array formula in cell A1
worksheet.Cells["A1"].SetDynamicArrayFormula("=B1:B3", new FormulaParseOptions(), false);
// Check if the cell contains a dynamic array formula
Console.WriteLine("Is A1 a dynamic array formula? " + worksheet.Cells["A1"].IsDynamicArrayFormula);
// Save the workbook
string outputPath = "DynamicArrayFormulaDemo.xlsx";
workbook.Save(outputPath, SaveFormat.Xlsx);
Console.WriteLine("Workbook saved with dynamic array formula at: " + outputPath);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
