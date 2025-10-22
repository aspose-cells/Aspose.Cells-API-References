##CalculationOptions.Recursive
CalculationOptions property. Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true
## CalculationOptions.Recursive property
Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true.
```csharp
public bool Recursive { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CalculationOptionsPropertyRecursiveDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Cells cells = wb.Worksheets[0].Cells;
// Create circular reference
cells["A1"].Formula = "=A2";
cells["A2"].Formula = "=A1";
// First calculation with Recursive=true (default)
CalculationOptions copts = new CalculationOptions();
copts.Recursive = true;
wb.CalculateFormula(copts);
Console.WriteLine("Recursive calculation result (A2): " + cells["A2"].Value);
// Second calculation with Recursive=false
copts.Recursive = false;
wb.CalculateFormula(copts);
Console.WriteLine("Non-recursive calculation result (A2): " + cells["A2"].Value);
}
}
}
```
### See Also
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
