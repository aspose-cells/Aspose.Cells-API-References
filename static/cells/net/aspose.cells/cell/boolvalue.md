##Cell.BoolValue
Cell property. Gets the boolean value contained in the cell
## Cell.BoolValue property
Gets the boolean value contained in the cell.
```csharp
public bool BoolValue { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyBoolValueDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
Cell cell = cells[0, 0];
// Set a formula that evaluates to a boolean value
cell.Formula = "=2.01>2";
// Calculate the formula to get the result
workbook.CalculateFormula();
// Demonstrate BoolValue property
Console.WriteLine("Cell BoolValue: " + cell.BoolValue);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
