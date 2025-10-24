##GlobalizationSettings.RowSeparatorOfFormulaArray
GlobalizationSettings property. Gets the separator for rows in array data in formula
## GlobalizationSettings.RowSeparatorOfFormulaArray property
Gets the separator for rows in array data in formula.
```csharp
public virtual char RowSeparatorOfFormulaArray { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class GlobalizationSettingsPropertyRowSeparatorOfFormulaArrayDemo
{
public static void Run()
{
// Create a new workbook with custom globalization settings
Workbook workbook = new Workbook();
workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();
Worksheet worksheet = workbook.Worksheets[0];
// Access the custom globalization settings instance
CustomGlobalizationSettings settings = (CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings;
// Display the current value of RowSeparatorOfFormulaArray
Console.WriteLine("Current RowSeparatorOfFormulaArray value: " + settings.RowSeparatorOfFormulaArray);
// Create an array formula using the custom row separator
Cell cell = worksheet.Cells["A1"];
cell.Formula = "=SUM({1,2|3,4})"; // Uses '|' as row separator
// Calculate formula to demonstrate proper parsing
workbook.CalculateFormula();
// Display results
Console.WriteLine("Array formula using custom separator: " + cell.Formula);
Console.WriteLine("Calculated result: " + cell.Value);
// Save the workbook
workbook.Save("PropertyRowSeparatorOfFormulaArrayDemo.xlsx");
}
}
// Custom GlobalizationSettings implementation overriding row separator
public class CustomGlobalizationSettings : GlobalizationSettings
{
public override char RowSeparatorOfFormulaArray => '|';
}
}
```
### See Also
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
