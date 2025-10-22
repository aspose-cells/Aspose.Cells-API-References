##Workbook.Settings
Workbook property. Represents the workbook settings
## Workbook.Settings property
Represents the workbook settings.
```csharp
public WorkbookSettings Settings { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookPropertySettingsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access and modify settings
workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
workbook.Settings.FormulaSettings.MaxIteration = 30;
workbook.Settings.FormulaSettings.MaxChange = 0.1;
// Verify settings
Console.WriteLine("Iterative Calculation Enabled: " +
workbook.Settings.FormulaSettings.EnableIterativeCalculation);
Console.WriteLine("Max Iterations: " +
workbook.Settings.FormulaSettings.MaxIteration);
Console.WriteLine("Max Change: " +
workbook.Settings.FormulaSettings.MaxChange);
// Save the workbook
workbook.Save("WorkbookSettingsDemo.xlsx");
}
}
}
```
### See Also
* class [WorkbookSettings](../../workbooksettings/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
