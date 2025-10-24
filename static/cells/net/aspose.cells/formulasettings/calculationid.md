##FormulaSettings.CalculationId
FormulaSettings property. Specifies the version of the calculation engine used to calculate values in the workbook
## FormulaSettings.CalculationId property
Specifies the version of the calculation engine used to calculate values in the workbook.
```csharp
public string CalculationId { get; set; }
```
### Remarks
This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. In the case of ms excel, if the value of this property is less than the recalculation engine identifier associated with the application that opens the resultant file, the application will recalculate the results of all formulas on this workbook immediately after loading the file. For performance consideration for most users' applications, we do not calculate any formula on the workbook automatically, no matter what value has been set for this property.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormulaSettingsPropertyCalculationIdDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Set formula that behaves differently based on CalculationId
Cell cell = sheet.Cells["A1"];
cell.Formula = "=AND(\"a\",true)";
// Calculate without CalculationId (default behavior)
wb.CalculateFormula();
Console.WriteLine("Without CalculationId: " + cell.Value);
// Set CalculationId and recalculate
wb.Settings.FormulaSettings.CalculationId = "181029";
wb.CalculateFormula();
Console.WriteLine("With CalculationId 181029: " + cell.BoolValue);
}
}
}
```
### See Also
* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
