##Cell.Calculate
Cell method. Calculates the formula of the cell
## Cell.Calculate method
Calculates the formula of the cell.
```csharp
public void Calculate(CalculationOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| options | CalculationOptions | Options for calculation |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodCalculateWithCalculationOptionsDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set a simple formula in cell A1
Cell cellA1 = worksheet.Cells["A1"];
cellA1.Formula = "=SUM(1, 2, 3)";
// Calculate with default options
cellA1.Calculate(new CalculationOptions());
Console.WriteLine("A1 value after calculation: " + cellA1.Value);
// Set an array formula in range B1:D1
Cell cellB1 = worksheet.Cells["B1"];
cellB1.SetArrayFormula("={1,2,3}", 1, 3);
// Calculate the array formula with options
cellB1.Calculate(new CalculationOptions());
Console.WriteLine("B1 value after calculation: " + cellB1.Value);
// Set a more complex formula in cell A2
Cell cellA2 = worksheet.Cells["A2"];
cellA2.Formula = "=IF(A1>5, \"Greater\", \"Less or equal\")";
// Calculate with options
cellA2.Calculate(new CalculationOptions());
Console.WriteLine("A2 value after calculation: " + cellA2.Value);
}
}
}
```
### See Also
* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
