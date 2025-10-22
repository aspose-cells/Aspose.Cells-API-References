##FormulaSettings.EnableCalculationChain
FormulaSettings property. Whether enable calculation chain for formulas. Default is false
## FormulaSettings.EnableCalculationChain property
Whether enable calculation chain for formulas. Default is false.
```csharp
public bool EnableCalculationChain { get; set; }
```
### Remarks
When there are lots of formulas in the workbook and user needs to calculate them repeatedly with modifying only a small part of them, it may be helpful for performance to enable the calculation chain. On the other hand, if the chain is enabled, maintaining the model of chain requires extra memory, and it also requires a bit more cpu time for some other operations such as changing cell's value or formulas. After changing this property from false to true, the calculation chain will be analyzed and built at the time of first calculation for the workbook, so the required time for the first calculation may be more than normal calculation without chain.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormulaSettingsPropertyEnableCalculationChainDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample formulas
worksheet.Cells["A1"].Formula = "=1+2";
worksheet.Cells["A2"].Formula = "=A1*3";
worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";
// Disable calculation chain
workbook.Settings.FormulaSettings.EnableCalculationChain = false;
// Calculate formulas
workbook.CalculateFormula();
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
Console.WriteLine("Workbook saved with calculation chain disabled.");
}
}
}
```
### See Also
* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
