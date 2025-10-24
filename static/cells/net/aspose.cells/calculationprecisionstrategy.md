##Enum CalculationPrecisionStrategy
Aspose.Cells.CalculationPrecisionStrategy enum. Enumerates strategies for handling calculation precision. Because of the precision issue of IEEE 754 FloatingPoint Arithmetic some seemingly simple formulas may not be calculated as the expected result. Such as formula 0.450.430.02 when calculating operands by  operator directly the result is not zero. For such kind of precision issue some special strategies may give the expected result
## CalculationPrecisionStrategy enumeration
Enumerates strategies for handling calculation precision. Because of the precision issue of IEEE 754 Floating-Point Arithmetic, some "seemingly simple" formulas may not be calculated as the expected result. Such as formula "=-0.45+0.43+0.02", when calculating operands by '+' operator directly, the result is not zero. For such kind of precision issue, some special strategies may give the expected result.
```csharp
public enum CalculationPrecisionStrategy
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No strategy applied on calculation. When calculating just use the original double value as operand and return the result directly. Most efficient for performance and applicable for most cases. |
| Round | `1` | Rounds the calculation result according with significant digits. |
| Decimal | `2` | Uses decimal as operands when possible. Most inefficient for performance. |
### Examples
```csharp
using Aspose.Cells;
using System;
namespace AsposeCellsExamples
{
public class CalculationPrecisionStrategyDemo
{
public static void CalculationPrecisionStrategyExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Formula");
worksheet.Cells["A2"].Formula = "=-0.45+0.43+0.02"; // This should ideally equal 0
// Set calculation options
CalculationOptions calcOptions = new CalculationOptions
{
IgnoreError = true,
Recursive = true,
PrecisionStrategy = CalculationPrecisionStrategy.Round // Using Round strategy
};
// Calculate the formulas in the worksheet
workbook.CalculateFormula(calcOptions);
// Get the result of the formula
double result = worksheet.Cells["A2"].DoubleValue;
// Output the result
Console.WriteLine("Calculated Result: " + result);
// Save the workbook
workbook.Save("CalculationPrecisionStrategyExample.xlsx");
workbook.Save("CalculationPrecisionStrategyExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
