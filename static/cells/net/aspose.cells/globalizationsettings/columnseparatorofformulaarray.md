##GlobalizationSettings.ColumnSeparatorOfFormulaArray
GlobalizationSettings property. Gets the separator for the items in arrays row data in formula
## GlobalizationSettings.ColumnSeparatorOfFormulaArray property
Gets the separator for the items in array's row data in formula.
```csharp
public virtual char ColumnSeparatorOfFormulaArray { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class GlobalizationSettingsPropertyColumnSeparatorOfFormulaArrayDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create custom globalization settings with overridden column separator
var globalizationSettings = new CustomGlobalizationSettings();
workbook.Settings.GlobalizationSettings = globalizationSettings;
// Display current column separator value
Console.WriteLine("Current ColumnSeparatorOfFormulaArray value: " +
globalizationSettings.ColumnSeparatorOfFormulaArray);
// Create array formula using custom separator
Cell cell = worksheet.Cells["A1"];
cell.SetArrayFormula("=SUM({1;2;3;4})", 1, 1); // Uses custom ';' column separator
// Verify formula storage (would show semicolons in actual formula string)
Console.WriteLine("Stored array formula: " + cell.Formula);
// Save modified workbook
workbook.Save("PropertyColumnSeparatorOfFormulaArrayDemo.xlsx");
}
private class CustomGlobalizationSettings : GlobalizationSettings
{
public override char ColumnSeparatorOfFormulaArray => ';';
}
}
}
```
### See Also
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
