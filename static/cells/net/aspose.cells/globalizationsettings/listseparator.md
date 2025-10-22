##GlobalizationSettings.ListSeparator
GlobalizationSettings property. Gets the separator for list parameters of function ...etc
## GlobalizationSettings.ListSeparator property
Gets the separator for list, parameters of function, ...etc.
```csharp
public virtual char ListSeparator { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class GlobalizationSettingsPropertyListSeparatorDemo
{
public static void Run()
{
// Create a new workbook with custom globalization settings
Workbook workbook = new Workbook();
workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();
Worksheet worksheet = workbook.Worksheets[0];
// Display current ListSeparator value from our custom settings
Console.WriteLine("Current ListSeparator value: " + workbook.Settings.GlobalizationSettings.ListSeparator);
// Create formula using custom list separator
worksheet.Cells["A1"].Formula = "=CONCATENATE(\"Hello\"; \" World\")";
worksheet.Cells["A2"].Formula = "=SUM(1;2;3)";
// Calculate formulas with custom separator
workbook.CalculateFormula();
// Show calculation results
Console.WriteLine("Concatenation result: " + worksheet.Cells["A1"].Value);
Console.WriteLine("Sum result: " + worksheet.Cells["A2"].Value);
// Save with formulas using custom list separator
workbook.Save("ListSeparatorDemo.xlsx");
}
private class CustomGlobalizationSettings : GlobalizationSettings
{
public override char ListSeparator => ';';
}
}
}
```
### See Also
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
