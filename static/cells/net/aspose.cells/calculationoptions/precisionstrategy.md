##CalculationOptions.PrecisionStrategy
CalculationOptions property. Specifies the strategy for processing precision of calculation
## CalculationOptions.PrecisionStrategy property
Specifies the strategy for processing precision of calculation.
```csharp
public CalculationPrecisionStrategy PrecisionStrategy { get; set; }
```
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CalculationOptionsPropertyPrecisionStrategyDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue(1.23456789);
worksheet.Cells["A2"].PutValue(2.34567891);
worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";
CalculationOptions calcOptions = new CalculationOptions
{
PrecisionStrategy = CalculationPrecisionStrategy.Round
};
workbook.CalculateFormula(calcOptions);
Console.WriteLine("A3 calculated value with Round strategy: " + worksheet.Cells["A3"].Value);
}
}
}
```
### See Also
* enum [CalculationPrecisionStrategy](../../calculationprecisionstrategy/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
