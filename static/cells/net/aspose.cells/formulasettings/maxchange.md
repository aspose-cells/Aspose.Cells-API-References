##FormulaSettings.MaxChange
FormulaSettings property. The maximum change to resolve a circular reference
## FormulaSettings.MaxChange property
The maximum change to resolve a circular reference.
```csharp
public double MaxChange { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormulaSettingsPropertyMaxChangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set up iterative calculation settings
workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
workbook.Settings.FormulaSettings.MaxIteration = 100;
workbook.Settings.FormulaSettings.MaxChange = 0.001; // Set maximum change threshold
// Create circular reference for demonstration
worksheet.Cells["A1"].Formula = "=B1+1";
worksheet.Cells["B1"].Formula = "=A1+1";
// Calculate formulas with the specified MaxChange setting
workbook.CalculateFormula();
// Output results
Console.WriteLine("A1 value: " + worksheet.Cells["A1"].Value);
Console.WriteLine("B1 value: " + worksheet.Cells["B1"].Value);
Console.WriteLine("MaxChange used: " + workbook.Settings.FormulaSettings.MaxChange);
}
}
}
```
### See Also
* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
