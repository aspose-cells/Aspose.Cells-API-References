##SettableGlobalizationSettings.RowSeparatorOfFormulaArray
SettableGlobalizationSettings property. Gets the separator for rows in array data in formula
## SettableGlobalizationSettings.RowSeparatorOfFormulaArray property
Gets the separator for rows in array data in formula.
```csharp
public override char RowSeparatorOfFormulaArray { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class SettableGlobalizationSettingsPropertyRowSeparatorOfFormulaArrayDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of SettableGlobalizationSettings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
// Display the default row separator for formula arrays
Console.WriteLine("Default RowSeparatorOfFormulaArray value: " + settings.RowSeparatorOfFormulaArray);
// Set a new row separator for formula arrays
settings.SetRowSeparatorOfFormulaArray(';');
// Apply the settings to the workbook
workbook.Settings.GlobalizationSettings = settings;
// Create an array formula in the worksheet
worksheet.Cells["A1"].SetArrayFormula("={1,2,3;4,5,6}", 2, 3);
worksheet.Cells["A2"].SetArrayFormula("=SUM(A1:C2)", 1, 1);
// Calculate formulas
workbook.CalculateFormula();
// Save the workbook
workbook.Save("PropertyRowSeparatorOfFormulaArrayDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
