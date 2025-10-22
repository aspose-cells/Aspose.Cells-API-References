##FormulaSettings.PrecisionAsDisplayed
FormulaSettings property. Whether the precision of calculated result be set as they are displayed while calculating formulas
## FormulaSettings.PrecisionAsDisplayed property
Whether the precision of calculated result be set as they are displayed while calculating formulas
```csharp
public bool PrecisionAsDisplayed { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormulaSettingsPropertyPrecisionAsDisplayedDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Set PrecisionAsDisplayed to true
workbook.Settings.FormulaSettings.PrecisionAsDisplayed = true;
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set display format for cell A1 to show 2 decimal places
cells["A1"].PutValue(1.23456);
Style style = cells["A1"].GetStyle();
style.Number = 2; // Format: 0.00
cells["A1"].SetStyle(style);
// Set formula in B1 that references A1
cells["B1"].Formula = "=A1";
// Calculate formulas with PrecisionAsDisplayed enabled
workbook.CalculateFormula();
// Output results
Console.WriteLine("A1 Display Value: " + cells["A1"].StringValue); // Shows 1.23
Console.WriteLine("B1 Calculated Value: " + cells["B1"].Value);   // Should be 1.23 due to PrecisionAsDisplayed
}
}
}
```
### See Also
* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
