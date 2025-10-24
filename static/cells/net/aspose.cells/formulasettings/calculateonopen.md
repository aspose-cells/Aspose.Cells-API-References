##FormulaSettings.CalculateOnOpen
FormulaSettings property. Indicates whether the application is required to perform a full calculation when the workbook is opened
## FormulaSettings.CalculateOnOpen property
Indicates whether the application is required to perform a full calculation when the workbook is opened.
```csharp
public bool CalculateOnOpen { get; set; }
```
### Remarks
This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormulaSettingsPropertyCalculateOnOpenDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set formula in cell A1 that references B1
worksheet.Cells["A1"].Formula = "=B1";
// Set value in cell B1
worksheet.Cells["B1"].PutValue(10);
// Disable automatic formula calculation on open
workbook.Settings.FormulaSettings.CalculateOnOpen = false;
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
// Reopen the saved workbook
Workbook reopenedWorkbook = new Workbook("output.xlsx");
// Verify formula wasn't calculated on open
Console.WriteLine("A1 value (should be 0 before calculation): " + reopenedWorkbook.Worksheets[0].Cells["A1"].IntValue);
// Calculate formulas manually
reopenedWorkbook.CalculateFormula();
// Verify formula was calculated
Console.WriteLine("A1 value (should be 10 after calculation): " + reopenedWorkbook.Worksheets[0].Cells["A1"].IntValue);
}
}
}
```
### See Also
* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
