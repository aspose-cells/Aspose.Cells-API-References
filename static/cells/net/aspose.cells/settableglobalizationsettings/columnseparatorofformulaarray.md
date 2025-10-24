##SettableGlobalizationSettings.ColumnSeparatorOfFormulaArray
SettableGlobalizationSettings property. Gets the separator for the items in arrays row data in formula
## SettableGlobalizationSettings.ColumnSeparatorOfFormulaArray property
Gets the separator for the items in array's row data in formula.
```csharp
public override char ColumnSeparatorOfFormulaArray { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class SettableGlobalizationSettingsPropertyColumnSeparatorOfFormulaArrayDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of SettableGlobalizationSettings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
// Display the current value of ColumnSeparatorOfFormulaArray
Console.WriteLine("Current ColumnSeparatorOfFormulaArray value: " + settings.ColumnSeparatorOfFormulaArray);
// Set a new value for ColumnSeparatorOfFormulaArray
settings.SetColumnSeparatorOfFormulaArray(';');
// Apply the settings to workbook
workbook.Settings.GlobalizationSettings = settings;
// Create an array formula with the custom separator using SetArrayFormula
worksheet.Cells["A1"].SetArrayFormula("SUM({1,2,3;4,5,6})", 1, 1);
worksheet.Cells["A2"].Formula = "=SUM(A1)";
// Calculate formulas
workbook.CalculateFormula();
// Display the result
Console.WriteLine("Result of array formula calculation: " + worksheet.Cells["A2"].Value);
// Save the workbook
workbook.Save("PropertyColumnSeparatorOfFormulaArrayDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
