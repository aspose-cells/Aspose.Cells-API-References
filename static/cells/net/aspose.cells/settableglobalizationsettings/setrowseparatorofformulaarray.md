##SettableGlobalizationSettings.SetRowSeparatorOfFormulaArray
SettableGlobalizationSettings method. Sets the separator for rows in array data in formula
## SettableGlobalizationSettings.SetRowSeparatorOfFormulaArray method
Sets the separator for rows in array data in formula.
```csharp
public void SetRowSeparatorOfFormulaArray(char c)
```
| Parameter | Type | Description |
| --- | --- | --- |
| c | Char | the specified separator |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class SettableGlobalizationSettingsMethodSetRowSeparatorOfFormulaArrayDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create custom globalization settings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
// Set the row separator for formula arrays to '|'
char rowSeparator = '|';
settings.SetRowSeparatorOfFormulaArray(rowSeparator);
// Apply the settings to the workbook
workbook.Settings.GlobalizationSettings = settings;
// Create an array formula in the worksheet
worksheet.Cells["A1"].SetArrayFormula("={1,2,3;4,5,6}", 2, 3);
try
{
// Calculate the formula to apply the settings
workbook.CalculateFormula();
// Display the formula with the new row separator
Console.WriteLine("Array formula with custom row separator: " + worksheet.Cells["A1"].Formula);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetRowSeparatorOfFormulaArray method: {ex.Message}");
}
// Save the workbook
workbook.Save("MethodSetRowSeparatorOfFormulaArrayDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
