##WorkbookSettings.FormulaSettings
WorkbookSettings property. Gets the settings for formularelated features
## WorkbookSettings.FormulaSettings property
Gets the settings for formula-related features.
```csharp
public FormulaSettings FormulaSettings { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyFormulaSettingsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access and modify FormulaSettings
workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Manual;
workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
workbook.Settings.FormulaSettings.MaxIteration = 100;
workbook.Settings.FormulaSettings.MaxChange = 0.001;
// Display the settings
Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);
Console.WriteLine("Iterative Calculation Enabled: " + workbook.Settings.FormulaSettings.EnableIterativeCalculation);
Console.WriteLine("Max Iterations: " + workbook.Settings.FormulaSettings.MaxIteration);
Console.WriteLine("Max Change: " + workbook.Settings.FormulaSettings.MaxChange);
}
}
}
```
### See Also
* class [FormulaSettings](../../formulasettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
