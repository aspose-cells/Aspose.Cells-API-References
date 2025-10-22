##Cell.GetFormula
Cell method. Get the formula of this cell
## Cell.GetFormula method
Get the formula of this cell.
```csharp
public string GetFormula(bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the formula needs to be formatted by locale. |
### Return Value
the formula of this cell.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodGetFormulaWithBooleanBooleanDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and formulas
Cell cellA1 = worksheet.Cells["A1"];
cellA1.PutValue(10);
Cell cellB1 = worksheet.Cells["B1"];
cellB1.PutValue(20);
Cell cellC1 = worksheet.Cells["C1"];
cellC1.Formula = "=A1+B1";
// Demonstrate GetFormula with different parameters
Console.WriteLine("Standard formula: " + cellC1.GetFormula(false, false));
Console.WriteLine("Local formula: " + cellC1.GetFormula(false, true));
// Change formula style to local and show difference
workbook.Settings.CultureInfo = new System.Globalization.CultureInfo("de-DE");
Console.WriteLine("Local formula after culture change: " + cellC1.GetFormula(false, true));
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
