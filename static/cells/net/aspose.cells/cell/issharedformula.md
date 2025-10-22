##Cell.IsSharedFormula
Cell property. Indicates whether the cell formula is part of shared formula
## Cell.IsSharedFormula property
Indicates whether the cell formula is part of shared formula.
```csharp
public bool IsSharedFormula { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyIsSharedFormulaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set shared formula in a range
worksheet.Cells["B2"].Formula = "=A2*2";
worksheet.Cells["B2"].Copy(worksheet.Cells["B3:B5"]);
// Check if cells contain shared formula
Cell cellB2 = worksheet.Cells["B2"];
Cell cellB3 = worksheet.Cells["B3"];
Console.WriteLine("Cell B2 IsSharedFormula: " + cellB2.IsSharedFormula);
Console.WriteLine("Cell B3 IsSharedFormula: " + cellB3.IsSharedFormula);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
