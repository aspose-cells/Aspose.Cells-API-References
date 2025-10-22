##FormulaSettings.ForceFullCalculation
FormulaSettings property. Indicates whether calculates all formulas every time when a calculation is triggered
## FormulaSettings.ForceFullCalculation property
Indicates whether calculates all formulas every time when a calculation is triggered.
```csharp
public bool ForceFullCalculation { get; set; }
```
### Remarks
This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormulaSettingsPropertyForceFullCalculationDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the formula settings
FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;
// Demonstrate ForceFullCalculation property
formulaSettings.ForceFullCalculation = true;
Console.WriteLine($"ForceFullCalculation is set to: {formulaSettings.ForceFullCalculation}");
// Add sample data and formula
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";
// Calculate formulas with ForceFullCalculation setting
workbook.CalculateFormula();
// Output the result
Console.WriteLine($"Calculation result: {worksheet.Cells["A3"].Value}");
// Save the workbook
workbook.Save("ForceFullCalculationDemo.xlsx");
}
}
}
```
### See Also
* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
